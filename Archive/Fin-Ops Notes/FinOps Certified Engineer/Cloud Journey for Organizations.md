## Traditional Technology Consumption

Traditionally, companies buying for the data center used platform or data center teams to gather requirements for hardware and software needed to support developers. These groups would create complex, often high-cost business cases, and would present them to procurement and finance groups for approval. If the business case was sufficient, procurement approved and gave them access to funding. 

There was a benefit to aggregating and standardizing purchases, and the size of the data center and availability of available funding put natural limits on what was spent. There were also process approval gates to be followed. Finance and procurement had easy visibility into costs and predictable invoices because they knew about every purchase before it was made. Resources were purchased in advance of demand, configured to run in the data center, and maintained there by full time staff, so, turning off or returning resources did not allow companies to save money.

**In this model...**

- DevOps, or engineers, are the requesters
- Finance and procurement are the gatekeepers, the approvers
- Spend is predictable and static, with known costs
- There are long procurement cycles
- The infrastructure purchased is usually intentionally oversized and not certain to be correct
- There is a high risk of failure to procure resources correctly to have a high cost.

## Along Comes Cloud

To complicate things further, in a DevOps world, there are many teams are working at once and technology requests are becoming more complex. Now, introduce the world of cloud and automation where procurement can be bypassed to make infrastructure purchases. This leads to companies where engineers with automation can spend money directly on the technology they need. Procurement and finance are losing control of the investment and the ability to track it over time. This means they cannot do their fiduciary duty to the company to control and correctly report on costs!

**Cloud changes the dynamic...**

- Engineers now have the power to spend company money with code
- Finance has less visibility into spend until after the fact and cannot do their fiduciary duty to the company
- Spend is dynamic and changes daily
- There is agile experimentation and some waste


## Operating Models of Consuming Cloud

Consuming cloud means costs are now highly variable and post invoiced. This is an entirely new experience for most roles at the organization. There are a couple different operating models that organizations will commonly use in the cloud. Each of these models comes with a different set of pros and cons.

### Centralized

In this model there is a central engineering team that performs cloud actions on behalf of the organization. 
**Implications:** Costs are clearly accounted for when all cloud actions are run through a centralized team. Change may be slower if many teams have requests all at one time. Limited innovation for roles outside of the central engineering team.

### Shared Platform
In the shared platform model there is a centralized team which offers a platform. The platform provides a layer of abstraction from the native cloud resources. Through this centralized team's tooling/APIs, teams across the organization are able to utilize the cloud based on the features and options made available by the platform. 
**Implications:** When this central group drives the rules of cost allocation and pushes out clear communication about how teams are doing, everyone is reassured that they’re being managed and measured against the same criteria. As engineers, you have the freedom to create within a given set of parameters.

### Fully Distributed
In this model all teams are able to access the cloud directly. Each team makes autonomous decisions and are expected to follow general guidelines around cloud use. In this model there may exist a Cloud Center of Excellence (CCoE). The CCoE may define which cloud services teams can use, tagging policies, access and permissions governance, etc.
**Implications:** This can be amazing at first glance. As an engineer, you have direct access to the cloud and merely an expectation to "be good." However, this can lead to lack of accountability, duplication of efforts, and over spend.

#FinOps 