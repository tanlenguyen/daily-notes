## Buy versus Build

There can be a significant effort to build automations and manage them going forward, especially with evolving cloud feature sets. Often, there are pitfalls along the way of building automation that you can only learn about as you go. In addition to building automation, you can also look at the buy option, or even consider a hybrid of the two. One benefit to the buying automation tooling is the vendors have most likely already coded for complexities and will keep up-to-date with Cloud service features. When deciding to build versus buy, consider the following questions.


1. Do you have the skills in house to build the automation?
2. What is the cost of building, but also maintaining the automation?
3. How long will it take you to get the automation in place versus buying an automation option and implementing?
4. If you buy an automation and it doesn't quite operate in the way you want it to, are you willing to build to augment?
5. Do you trust the security of your platform to the security of a vendor platform?

## Getting Started

You're ready to start automating, but you shouldn’t try to implement too much automation all at once. This will inevitably cause issues and have you struggling to make sure the automation you deploy is working effectively. Here are some tips:

- **Start simple -** Start with a simple selection of tools and automation goals. Trying to build a very complex set of automations and/or coordinating multiple sets of tools all at once will often lead to unnecessary challenges.
- **Use it in an inform mode first -** Start initial automation in an inform mode, automating the discovery and alerting of potential issues, but not their remediation, so it lets you know what it would do if it were enabled to make changes.
- **Build confidence in the automation** - Learn about the actions an area of automation will take once it is enabled. Build confidence by sharing the results with your team and FinOps practitioner to ensure they are comfortable with the introduction of automation.
- **Do lots of testing** - Once you've built confidence with automation, start enforcing actions in dev/testing accounts first and then test with smaller groups before broadening to a wider user base.
- **Don't build it all yourself** - It's okay to rely on commercial or open source tools. Not only will this save time, but it will also make sure you get the latest battle-tested solutions.
- **Measure the performance** - Automation should be measured to ensure it is having the desired effects. As automation is scaled out across the organization, it is essential to measure that the performance is not degrading.

## Collaboration with FinOps

FinOps practitioners are looking to help you with automation. Some automation will be very specific to the way your organization operates, but there are also some common automation solutions that your FinOps team will look to implement. 


**Tag Governance**

Once a tagging standard is defined for your organization, your FinOps champion will start looking to automation to ensure it is being followed. This will most likely involve identifying resources with missing tags or incorrectly applied tags and then having those responsible (you) for the resources address the tagging violations. If you think this is about to be implemented, or it has already been implemented at your organization, you can collaborate with FinOps to better understand the tagging standards. This might even be an opportunity for your to create your own automation to tag certain resources. 

**Scheduled Resources Start/Stop**

Resource management and automation enables you to schedule resources to be stopped when not in use (e.g., while you’re away from the office) and then have them brought back online when you need to use them again. The goal for this automation is to minimize impact on teams while realizing large amounts of savings for the hours that their resources are shut down. This automation is often deployed into development and test environments, where the absence of the resource isn’t noticed outside of business hours. Work with your FinOps practice to ensure you are able to skip scheduled activities (in case you are working late) or cancel a scheduled task (the resource should not be removed from the automation, just skipped). 

**Usage Reduction**

The FinOps practice may decide to implement reduction automation. This automation removes waste, or at least sends alerts to responsible staff members (you) to drive better cost optimization. When you receive these alerts, it is time to investigate or, within some environments, to autostop or resize the resources.

## Automation Framework

[(opens in a new tab)](https://www.youtube.com/watch?v=TD3EqFO46HE&list=PLUSCToibAswlUXVZX2caukPWYzkDc597D&index=15)In the video below, learn more from Bindu Sharma, Senior Manager, FinOps. Bindu started her career as a software engineer and is now a FinOps practitioner. In this video, learn more about how FinOps will be looking to collaborate with you throughout the automation process.

## Conclusion

[(opens in a new tab)](https://www.youtube.com/watch?v=TD3EqFO46HE&list=PLUSCToibAswlUXVZX2caukPWYzkDc597D&index=15)Let's recap on automation. When you have a repetitive task that needs to be performed often, automation removes the effort and maintains consistency. When deciding to automate, consider the outcome and be sure to validate that automation is the correct solution. Next, watch for automation conflicts and be sure to monitor automations over time. And, lastly, partner with FinOps to make automation decisions.