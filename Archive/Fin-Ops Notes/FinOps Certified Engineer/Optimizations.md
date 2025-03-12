
## Optimzation Levers

While we need to focus ultimately on the value we get from our cloud spending, we do have to focus sometimes on cost. Optimization is about reducing the cost part of the value equation and managing the cost arm of the iron triangle. 

When looking at the cloud spend formula there are two levers we can pull to optimize. **We can either reduce the rate or reduce usage.** However, let's be clear: FinOps is not just about saving money. FinOps is about balancing the conversation back to the iron triangle and tradeoffs to make sure you are maintaining value and at the same time driving efficiency. If you can reduce costs without impacting quality and speed, then you are creating efficiency. However, if you are impacting quality or speed then the value costs need to be discussed.

## **Rate Optimization**

Optimizing rates is the job of the central team. Rate optimization is best done when looking holistically at the organization's cloud usage. Although the specifics can vary greatly by vendor and service, discounting in general is similar regardless of vendor or type. Commitment to the cloud provider—in terms of dollars, time, and specific cloud usage—will get you discounts. The more specific, the larger, or the longer your commitments, the more you can generally save.

Cloud providers discount because they want predictability (the same as private data centers, but with more scale). Discount programs at CSPs don't care if a commitment—for example on compute—is used by your service or some other service in your organization. Your FinOps practice will look for a consistently used amount of resources to purchase commitment discounts, and will consider your team's usage with everyone else's to determine what to purchase. And, because you are committing to pay, you are by definition giving up flexibility that on-demand service usage offers. The other way to think about this is the cloud providers are buying your flexibility. Despite the fact that this is scary, do not wait. Constantly work on getting discounts. 

For example, one team at your organization may have high resource usage during the day while another has high resource usage during the night. Based on their usage, it probably doesn't make sense for either team to make commitments individually. But, overall, there is a consistent base of resources running across the 24-hour period. FinOps has identified the opportunity to commit to a reservation and save both teams on the rate they pay for resources.

Understanding the holistic view of cloud spend and making decisions around discounts and commitments is complex. There are many options available and some options will work together, while other options will not. With this hugely complex task, a centralized team is needed to view rate and usage holistically to balance these together.

**To pull this lever, you will partner with FinOps who is operating this large scale rate optimization.** FinOps will be looking to you to help understand where you can make locked in commitments and where you cannot be locked in. Once the organization commits to a Cloud Service Provider (CSP), you will be locked in to that type of usage over time. The more consistent you are around usage of cloud, then the more likely it is that discount programs can be used. FinOps may be the owner of rate optimization, but it is your responsibility to look at your usage to determine where flexibility can happen and where you can commit to locked in rates.

## **Usage Optimization**

Usage optimization means optimizing the actual resources you are deploying and managing which account for cloud usage. You, the engineer, are the owner of usage optimization. It is probably unlikely that you would want someone else to go and change your actual resources, so this optimization lever belongs to you. Luckily, FinOps is here to partner with you on this optimization effort as well. The FinOps champion will be responsible for identifying optimization opportunities and sharing them with you. Then, you own the opportunity and must put time in your schedule to test, validate, and execute. 

Usage optimization is not a one-time fix but a continuous cycle of picking properly sized resources and eliminating overprovisioning. Usage optimization requires you to think of cost, just like you think of memory and bandwidth: as another deployment KPI. Initially, usage optimization may be retroactive. You'll go through and clean up infrastructure to ensure a fully utilized set of resources. However, over time, you can begin to proactively consider cost in architecture reviews before deployment and actively consider cost when choosing cloud resources at the start.

The goal is not to make the perfect decision. It’s to make the best decision possible given the context and data, and then reevaluate often. A well-sized resource won’t stay that way forever, as code and load evolve over time.

### **Candidate for Optimization**

As mentioned, the FinOps practitioner is going to identify optimization opportunities. They will look for a mix of easy wins and harder elements. Most optimization candidates will fall into one of the four categories below. 

|   |   |
|---|---|
|**Potential Savings**|**Optimization Opportunity**|
|**Avoid 100%**|Find and eliminate or turn off unused things|
|**Save 50%**|Commit to consistently used resource usage|
|**Save 25%**|Rightsize or modernize|
|**Save 1-100%**|Use different things to deliver the same value|

Below is a potential list of optimization opportunities. They are more or less in order of difficulty. Some of these are slightly more concrete examples of optimization opportunities your FinOps practice may pursue. 

- Turn off/turn on development, test, sandbox environments    
- Create/manage storage policies to deprecate storage over time to cheaper tiers    
- Rightsize compute, databases, networks, environments     
- Change from 3rd party licensed resources to cloud native resources    
- Modernize resources    
- Service substitution (or license substitution)    
- Mature your DevOps approach     
- Move to/expand use of containers    
- Move to serverless    

Depending on your organization, the FinOps champion may bring one or many optimization opportunities to you. Remember, it is your responsibility to test, validate, and implement optimizations that bring the most value to the business.

## **Your Role**

Both rate optimization and usage optimization require a partnership between you and your FinOps team. This partnership can be mutually beneficial to help you get the most value out of your cloud spend. Additionally, FinOps champions are often well-known throughout the organization and talk to key leaders. Working with them can help get your name out for wins in the area of maximizing value and efficiency! 

_The table below outlines the roles you and your FinOps partner play in optimization efforts._

![[Pasted image 20240809143623.png]]

## Informed Ignoring

Within the optimization efforts, you may be brought many opportunities to save. As mentioned before, it is your role to test and validate opportunities and possibly execute. Before taking action, you must weigh the value of executing each optimization opportunity against the value from other priorities. For example, you might find that delivering a feature on your roadmap returns more value than an optimization opportunity at this time. From that, you can have confidence when deciding to continue with the current trajectory and hold off on the optimization opportunity for now. 

**There is a big difference between being informed on opportunities and choosing not to execute versus totally ignoring and not identifying and measuring opportunities at all.** 

If you choose to totally ignore an opportunity, then you lose the ability to assess the value of the optimization compared to what you are working on now. Often this is paired with the sentiment that as an engineer you don't need to worry about the cost also known as deep pocket syndrome. Think back to the Data module of this course. We talked about whether you're building a race car or a family sedan. When building, without constraints, the race car of clouds, your future is likely to include "Oh, I wasn't expecting it to cost that much."

With informed ignoring, you are shown an opportunity to test and validate and then you have the option to ignore the opportunity if there are other efforts of higher value that take priority. If you decide something is not worth your time to do, you do not ignore it forever, you set it aside and revisit it on occasion to see if it is a good idea at that time. This informed ignoring also means the business is informed. The opportunity was evaluated and decided that other efforts take priority. This way the business knows what is coming so ideally you don't have some form of emergency cost reduction, redo of work, quick patching, etc. Being informed is a good thing, it will only make you better able to engineer.

## The Action Scale

The action scale below depicts how likely someone is to take action. There are both contributors and detractors to action. 

- **Contributors** - interest, motivation, understanding
- **Detractors** - effort and time, process, risk

### **Why It Matters**

When optimization opportunities arise, FinOps champions will partner with you to help tip the scales toward action rather than inaction. It may feel like another person is putting a constraint or request on your time, however, this partnership can greatly benefit you as an engineer. 

For example, FinOps comes to you with an optimization opportunity. Here are a couple of types of requests you could make of them. 

- Can you do this part of the request to reduce the lift and effort on my end?
- Can you get the preapprovals needed from the business?
- Can this change request be put into our change request template? 
- Can you vet these recommendations and pick only ones that are material enough? 

With these types of requests, effort and time on your end are reduced, and maybe your motivation to take action increases. Additionally, it is okay to seek to understand why a FinOps champion is asking you to do something. Then, after testing and validating the opportunity you can both discuss the value, weigh this value against existing work, and decide on the best path forward. This means that you've done your due diligence, everyone is informed, and the business gets maximum value out of their cloud spend!

#FinOps 