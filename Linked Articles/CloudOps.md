
When adding [[QuickSight]] users to Admin, be sure to share all datasets with them too. 

IAM Identity Center for all SSO and Permission sets for accounts that need access. 

There is a button called "Simulate" on every IAM role, that will lead to the simulator.

# Removing disabled users
At this point our standard operating procedure for these adhocs should be:

  - login to Stuller Technology Master console

  - make sure you are in us-east-2 region

  - search for the user in AWS IAM Identity Center (make sure it isn't regular IAM)

       - make sure to use Display Name as the search field not Username

  - if the user does pull up

         - click on the username

         - click the Groups tag

         - if any of the groups are admin groups, send a Teams message in this chat letting me

# Kubernetes
K9s for logging and observability.
Installation is done manually through a curl and we get the latest then install it from there.


# CloudWatch

## Cost anomalies in EBS 
cloudwatch->Logs Insights->Select DataProduction-vpc-flowlogs, and typed into the query generator