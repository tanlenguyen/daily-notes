Checking Splunk for any increase in items with the following inquiry:

```
index=aws-logs data_manager_input_id="76d1047f-a28c-4bb3-9b20-ad2991ba08a4" OR source="*_76d1047f-a28c-4bb3-9b20-ad2991ba08a4" aws_account_id=168806633334 userAgent="config.amazonaws.com"
```

