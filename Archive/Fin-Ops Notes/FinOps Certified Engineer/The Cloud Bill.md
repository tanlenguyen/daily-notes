## **Billing Data Complexity**

One of the challenges an organization faces is the massive amount of information presented in the cloud bill. Previous to the cloud, billing included invoices for planned purchases like equipment and hardware. Now, the pricing of the services consumed within the cloud is presented in a complex mix of charges. 

As an engineer, it is important to have an understanding of cloud billing. If you are asked to explain anomalous spend or predict future spend, then you'll be faced with the complexity of how cloud providers charge for different services and how these costs are represented in the cloud bill. This will all boil down to a single equation. 


Usage might be the number of seconds a resource is used (e.g. virtual machines) or the amount that is consumed (e.g. storage). The rate is the amount paid per unit of usage of that resource. Conceptually, it’s pretty simple. Change either of those items and your cloud bill goes up or down. Increase both and it can go way, way up.

Cost for individual cloud resources may seem relatively inexpensive, but at scale across many engineers over time will add up to significant amounts of spend. Being cost-aware and intentional with your infrastructure choices will help avoid out of control costs. 

When working with FinOps practitioners or finance partners, remember that low hanging fruit won't necessarily be a big apple. Even a small change, saving a couple cents a month, can lead to large savings in the long term.


## **A Month is Not a Month**

Cloud billing is all about time! Cloud billing doesn't use a fixed month like many finance teams are used to. Imagine your company has adopted a new cost optimization initiative at the beginning of the year. It starts off on January 1 with a list of cost-cutting actions including turning off some unused instances, rightsizing others, and purchasing some Savings Plans. The following month, the cloud bill drops 10%. Success!

But wait. If you divide the number of days in February by the number of days in January, you get 90%. That may seem painfully obvious, but you can’t even begin to count the number of times that the change between February and other months has falsely convinced a team that they’ve been effective in reducing costs. Then, inevitably, on March 31, there’s a panic because costs are up 10% month over month.

This time element plays into effect in cost and billing particularly when predicting costs in something less than 365 days. Traditionally, finance was given an annual bill that was divided evenly into 12 months. Now, friction can exist between finance and engineers because finance isn't expecting an increase in spend just because the month is longer. As an engineer, being aware of time as part of the cost/spend formula is crucial. 

Remember: (Time or Usage) x Rate = Cost.

#FinOps 