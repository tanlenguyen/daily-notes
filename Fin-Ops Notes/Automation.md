## Automation

As we just discussed optimization and driving value from cloud, automation may be one way to reduce effort and maintain consistency.

### Benefits 

Creating an automation might not reduce effort (the amount of time to automate might be the same amount of time to do the task), but it drives consistency and reliability of the actions being taken.

- **Drive up reliability**- rather than an individual trying to remember to complete a task at a given frequency, automation can step in and the task will be consistently completed (even if the individual is on vacation, out sick, or just forgets to do the task)
- **Increase consistency** - automation can help ensure an action is done the same way every time

### Drawbacks

There are lots of activities happening in a cloud environment. Automation will require you to be informed of these and what is taking place so that you are not surprised if the automation doesn't go well or the risks are too high. 

- **Set it and forget it** - if an automation is running and doesn't go well, it could impact a whole range of things. If you didn't notice this, the automation could very well take out your service and become a major issue
- **Managing risks** - with automations, extra time is needed to ensure that the risks of automation errors are managed within the organization
- **Level of permission** - automation requires a level of permission into your cloud environment in order to be taking action; this risk and compliance element should be considered when implementing automation

To automate or not to automate? That is the question. You can determine the answer by looking at two aspects of your organization. First, you must outline the outcome you want to achieve with automation. Second, you need to compare automation to a manually tracked process within the organization and determine whether automation is a better method to achieve the desired outcome you’ve identified. 

Should you automate? Ultimately, the answer is “it depends,” as is often the case. To answer the question, we must look to the benefits achievable from automation.

### Automation Outcomes

When choosing to automate, first identify the actual business outcome (not just the way the automation will achieve that outcome). For example, if you take a look at idle resource governance, you could be forgiven if you think the goal is to remove idle resources from your cloud environment. But in reality, the outcome is that you want to remove the costs of these resources because they’re costing you money. This is important, because you use such goals to measure the performance of your automation. Once you have a business outcome in mind, it is time to decide if the outcome can be achieved via automated versus manual tasks.

### *Automated Versus Manual Tasks**

In this second step, you want to validate that automation will help you deliver on the outcome or goal. Sometimes, the effort of automating (which may exceed the effort of doing the task manually) can still be worth it. As humans, we make mistakes, and automation can be used to correct them. 

A great example of using FinOps automation to reduce errors and effort is when you automate the process of adding supplementary tag data to resources. Your team may tag their resources with a simple identifier and then have automation add extra, clarifying tags based on the correlation between that identifier and an outside data source like a CMDB. Your team might use a project identifier that maps to cost centers or to environment types, or to have the project identifier tag itself be automatically identified from the outside CMDB based solely on the identifier. Automation would find that project identifier, add the extra tags to the resources, deliver the relevant cloud spending data to your team’s systems for display or future automation, and generate cloud spend reports such as anomaly alerts. This reduces the number of tags you need to apply, avoids human error, and makes sure that the extra tag data is applied in a consistent manner, then delivers that data into your hands. 

When trying to work out how much time and effort it takes to add automation versus how long it takes for you to do the thing, look for an ROI (return on investment). Looking at the chart below from [xkcd.com(opens in a new tab)](http://xkcd.com/), if you have a task that takes you 1 minute to perform and you do this task once every week, over 5 years you will save a total of 4 hours if you automate the task away. So unless it takes you less than 4 hours to setup and maintain the automation, you will not be saving time. However, you might be willing to take a hit in time-to-build if the consistency of the task being done by automation is crucial. Remember, one major benefit of automation is the task will be completed the same way, every time.


## Continuous Improvement

There are many reasons to reassess automation decisions and automations currently in place over time. For example, your organization's cloud footprint may grow and what initially didn't make sense to automate, may now prove worthwhile at scale. Or, conversely, something you did automate initially may be more complex to manage or troubleshoot that expected, causing a temporary move back to a manual process. There is also the consideration of new tooling that offers some automation as part of a package. You will need to continue, over time, the cost-benefit analysis of adding and maintaining automation.