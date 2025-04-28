# AWS to Azure
https://learn.microsoft.com/en-us/azure/architecture/aws-professional/

When adding [[QuickSight]] users to Admin, be sure to share all datasets with them too. 

IAM Identity Center for all SSO and Permission sets for accounts that need access. 

There is a button called "Simulate" on every IAM role, that will lead to the simulator.

# Adding User to a group
1. Check to add user to AD user group. 
2. Go to IAM Identity Center
3. Multi-Account Permissions->AWS accounts.
4. Find the Account the User needs access to
5. Add the level of permissions needed then add the user to the account
6. Wait 10 mins, and close the ticket after giving permissions

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

# Calculation

The percent change can be calculated using the formula:
$$
Percent Change = (New Value - Old Value)/ Old Value​×100
$$


# Website Infrastructure
Digital does not scale with traffic, so no elastic load balancers with the website


#FinOps #CloudOps 