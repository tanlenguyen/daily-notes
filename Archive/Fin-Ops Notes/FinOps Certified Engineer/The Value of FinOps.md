## Collaboration

What is the return on investment for you, as an engineer, in making these trade-off decisions and collaborating with your FinOps champions? The FinOps practitioner can guide you through assessing decisions, setting expectations, and validating results. For example, a FinOps practitioner might provide guidance by adding a cost management perspective, or they may be able to provide visibility across the organization and can assist in validating business value.  This persona is a critical resource and it is important to build a relationship with them to help you get the most out of their expertise.

### **Assessing Different Scales of Decisions**

This is the Iron Triangle in action! When making this assessment, you will need to include personas depending on the scale of the decision. For example, decisions with small variations in cost impact will happen within your engineering team itself (this may depend on what your organization caps as the amount this could be within). 

For other decisions, you will work directly with your FinOps practitioner to assess the scale impact of the change and then figure out who needs to be involved (the bigger the number, the more personas needed to make the decision).

As an example, you may want to use a more specific database that is tailored to your workload. This increases your cost by a few percent and is within your authority to decide. However, you might decide to add a read replica of your data because it will dramatically improve performance, but this would increase your data cost by 30%. In this case, you would likely need to include the product owner and finance in the decision to ensure everyone is okay with this trade-off of cost and quality. Later, you may decide to make your application fully multi-location, replicating more aspects of the system into multiple regions. This type of change entails millions of dollars of investment, weeks or months of work, and impacts to both cost and speed to increase quality. This decision may still be justified because it will drive sales into a new market or support price increases that outweigh the cost, but this decision would likely involve personas from engineering all the way to the CTO/CIO. 

Work within your organization to understand where the thresholds for different scale decisions are on all three arms of the iron triangle. Knowing that you have the authority to make decisions in areas where costs are impacted by less than x% of your application cost, or time is impacted by less than y hours in any sprint, gives you more freedom to operate, and the knowledge to know when you should collaborate. Additionally, taking the time to assess the scale of a decision and the right people to involve, will get everyone on the same page. This means, when the costs come through, everyone will be aligned on the value of the decision that was made.

**The Iron Triangle (quality, speed, cost)  is not just for large scale decisions. It can also be used in smaller day-to-day decisions within your team.**

### **Proactively Setting Expectations**

Now that you have decided which personas must be involved in making a value-based decision, it is time to set expectations. Working with your FinOps champion and any other personas involved, the conversation around trade-offs and value-based decisions can begin. These conversations set the stage for other personas (finance, leadership, etc.) to better understand cost impacts of new designs, changes in architecture, or even service code updates. And, you are able to justify decisions and refer back to these expectations throughout the life of the project.

### **Validate Results**

You've now assess the decision, involved the right people, worked to set expectations, and implemented the solution. Next, it is important to validate the data from the bill to understand the cost impact. This is where the FinOps champion can support! 

Sometimes, a cost impact will not be directly felt by the team who made the decision. A seemingly low-cost decision for your team, might generate costs for another team. The FinOps practitioner has visibility across the organization and can help validate results and cost impact.

For example, let's think about security. You might spin up and tear down free cloud resources because there is zero or little cost impact. However, there is security tooling that is monitoring all of the resources being created and deleted. With all of your spun up resources, their costs go up. So, rather than just validating the impact of your decisions within your team, the FinOps practitioner well help look at cost impacts wholistically across the organization. 

If a FinOps champion comes to you about costs, remember that you may have impacted your costs, but another team may have as well. Work together to figure out what is changing. You may find out that your team was not the catalyst for where spend is going up.

## It's Worth It! 

Let's recognize that this is a lot of work outside of actually doing the engineering. You are now being asked to analyze decisions, collaborate with FinOps, make trade-offs, implement solutions, validate results, and even support in understand cost impacts with other teams. Ultimately, although this may seem like a lot of work, it will lead to more freedom within the actual engineering portion of your role. By knowing the expectations and aligning on trade-offs, you will be able to craft a solution within those parameters with less fear of rework or even upset stakeholders. 

Lastly, make friends with your FinOps champion. They will be the one to support you and your team through all of this! They are often well known across an organization and can be an excellent resource. Taking advantage of their support and committing to having trade-off conversations to make value-based decisions is well worth it!

#FinOps 