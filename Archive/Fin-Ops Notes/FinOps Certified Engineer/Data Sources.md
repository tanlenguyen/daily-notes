## **Cloud Spend & Pricing Data Sources**

In addition to understanding the cloud bill, there are common data sources that are part of a FinOps practice data workflow. Below is a list categorizing of one of the primary sources of accurate data needed within FinOps. However, acquiring this dataset involves ingesting data from various cloud providers using multiple mechanisms, such as retrieving CUR files from AWS S3 buckets for object storage or utilizing APIs for Azure, among others. It is crucial to recognize that different cloud providers offer diverse billing programs, resulting in varying methods of accessing billing data. For instance, in Azure, the endpoints and API schemas for billing data APIs differ depending on the program, whether it's PAYG, Azure EA, or Azure CSP. It is important to have reliable data workflows to address these diverse feeds of data.

You may work with those in your organization's FinOps practice to understand this data and to confirm that the data queries you are running are being interpreted accurately.

### **Public Cloud Billing**

This is the core dataset from a FinOps perspective. It contains the detailed, granular consumption and billing information that can be used to form a picture of consumption and cost for most cloud services. It can also be enriched with tagging metadata to enable mapping to other key datasets within your organization. At a minimum, public cloud billing data will include:

- Cloud account identifiers
- Date (time granularity can be configurable in some cases)
- Resource hierarchy (i.e. accounts, subscriptions, projects, resource groups, tagging metadata)
- Cloud technology types (e.g. storage, compute, database)
- Part numbers/metering information
- Consumption quantities
- Price per service SKU
- Consumption cost
- Charge Type
- Individual resource identifiers
- Discount information

### **Public Cloud Pricing**

The price sheet contains the details about a cloud provider’s rates for its services.  Rate information contained within these files include both on-demand rates as well as rates for commitment-based discounts.
### **Public Cloud Tagging**

Tagging is metadata which provides additional granularity to billing reporting that can enable mapping to other key datasets within your organization. Maintaining clean tagging data is critically important for accurate and reliable reporting. Tagging policies, enforcement, provisioning strategies and third party tools can help with maintaining and normalizing tag data; especially for multi-cloud organizations. The tags and associated values applied to a cloud resource, accounts, resource groups, etc. can feed into the Public Cloud Billing data. However, not all tags on cloud resources appear in the cloud billing data, gathering the full set of tags associated with cloud resources can add further context/details to the use/value of the resource.

### **Configuration Management Database**

Configuration Management Databases (CMDBs) are used to store IT configuration records and the relationships between them. They are generally populated via a combination of automated and manual processes and are intended to be used as the ‘source of truth’ for IT configuration information within an organization. The reality is that CMDBs are only as good as the data feeds and processes used to manage them, so before incorporating CMDB datasets into a FinOps data model, the quality, accuracy and timeliness of the data must be assessed.

The primary use-case of CMDB data in a FinOps dataset is Application and Service data. A well managed CMDB will be the source of truth for data such as Application and Service names, ownership, organizational alignment, criticality, and hours of operation. This data can provide the crucial link between cloud consumption, applications and people.

CMDBs can also maintain records of public cloud configuration via automated and regular data feeds, however the source of truth for this type of data is always going to be the cloud platform itself. 

CMDB Application and Service data can be used to populate resource tags on a cloud platform, which is in turn incorporated into the dataset by way of the cloud billing data, eliminating the need for a direct feed from the CMDB. This approach may be also implemented for non-FinOps use-cases such as enabling self-describing cloud resources to support operations and automation activities.

### **Finance Cost Centers**

A cost center represents the smallest segment of an organization for which you collect and report costs (project, team, department, etc.). 

Only a small number of segments within an organization are revenue or profit centers. Some are cost and profit centers at the same time. The organization determines whether to set different codes for cost and profit centers.

### **Org Tree / Staff Lists**

In traditional organizational structures, the Org Chart (or Org Tree) is a visual representation of the organization where employees are grouped by function, region or product line. The staff list provides information on span of control, chain of command and general information at employee-level (contact information, time zone, geography). The staff list is a living and breathing document, unlike the org tree which may not get updated in real time. These lists can be important when attributing costs to heads of areas and can be an effective way to drive FinOps practices and cloud accountability.

### **Budgets (Cloud Spend)**

Cloud spend budget should be prepared prior to the start of the business cycle, with a supplemental budget or budget revision prepared as needed based on changing business conditions.

Of the many common budgeting methods, the two most efficient to build and maintain are incremental and activity-based budgets. Cloud spend aligns better to activity-based budgets, albeit the activities can move very fast and grow into a large number of activities within a very short amount of time resulting into significant and unexpected cloud expense if not actively managed.

### **Performance & Utilization Data**

Organizations can gain valuable insights and achieve cost savings by establishing data workflows to capture utilization data across various metrics and cloud resources. This data is vital for understanding resource utilization, optimizing resource allocation, and improving cost efficiency.

Data workflows should cover a wide range of cloud resources, including virtual machines, storage volumes, databases, and containers. By capturing metrics like CPU utilization, memory usage, and network traffic, businesses can analyze utilization trends, identify inefficiencies, and make informed decisions. These decisions may include right-sizing instances, eliminating underutilized resources, and leveraging cost-saving opportunities such as reserved instances or committed use discounts offered by the cloud provider. 

In summary, establishing data workflows to capture utilization data across different metrics and cloud resources is crucial for organizations to gain insights, optimize resource allocation, and achieve cost savings. By making informed decisions based on this data, businesses can maximize their cost efficiency in the cloud environment.

#FinOps 