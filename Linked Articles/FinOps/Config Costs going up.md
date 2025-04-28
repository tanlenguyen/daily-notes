# Checklist
1. Checking Splunk for any increase in items with the following inquiry:

```
index=aws-logs data_manager_input_id="76d1047f-a28c-4bb3-9b20-ad2991ba08a4" OR source="*_76d1047f-a28c-4bb3-9b20-ad2991ba08a4" aws_account_id=168806633334 userAgent="config.amazonaws.com"
```

2. Check the following link: https://serebrov.github.io/html/2019-10-08-aws-config-charges.html for anything that might be going on.
	1. Use the following table:
	`CREATE EXTERNAL TABLE awsconfig (`
    `fileversion STRING,`
    `configSnapshotId STRING,`
    `configurationItemVersion STRING,`
    `configurationItemCaptureTime STRING,`
    `configurationStateId BIGINT,`
    `awsAccountId STRING,`
    `configurationItemStatus STRING,`
    `resourceType STRING,`
    `resourceId STRING,`
    `resourceName STRING,`
    `ARN STRING,`
    `awsRegion STRING,`
    `availabilityZone STRING,`
    `configurationStateMd5Hash STRING,`
    `resourceCreationTime STRING`
`)`

`ROW FORMAT SERDE 'org.apache.hive.hcatalog.data.JsonSerDe'LOCATION 's3://aws-controltower-logs-571694804400-us-east-2/o-gvhvixx128/AWSLogs/168806633334/Config/us-east-1/'TBLPROPERTIES ('has_encrypted_data'='false');`

Change the dates

`SELECT result.configurationItemCaptureTime,`
       `COUNT(result.configurationItemCaptureTime) AS NumberOfChanges`
`FROM (`
      `SELECT regexp_replace(`
                `configurationItemCaptureTime, '(.+)(T.+)', '$1'`
             `) AS configurationItemCaptureTime`
      `FROM s3data.awsconfig`
      `WHERE "$path" LIKE '%ConfigHistory%'`
        `AND configurationItemCaptureTime >= '2024-05-01%'`
        `AND configurationItemCaptureTime <= '2024-06-28T%'`
     `) result`
`GROUP BY result.configurationItemCaptureTime`
`ORDER BY result.configurationItemCaptureTime;`

3. f

# Preventative Measures
Putting Cost Anomaly alerts on the resources discovered from the Athena queries would help. In some rare cases it might be worth it to put weekly and daily alerts on in case of rates of increase. 

#FinOps #CloudOps 