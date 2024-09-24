## Data-Driven Decision Making

Within your organization and your role, there are many decisions to be made. You can utilize the iron triangle to support trade-off conversations, but you will always need data to prove that the decisions you make are driving value to the business.

The nirvana state of FinOps is when everyone can make collaborative, data-driven decisions that create value. This means you—engineering teams—need to make efficient choices every day, not just when there's a mandate. Leadership can define and support using cost and sustainability metrics as first class requirements alongside other traditional DevOps metrics. However, the goal is to get to a place where you have the data to build, run, and optimize continuously to drive business value.

- **For architects** cost informed data-driven decisions are most impactful when designing infrastructure
- **For engineers** cost informed data-driven decisions are most impactful when writing code and deploying services


It is an ongoing collaborative effort to make data-driven decisions focused on maximizing business value. This can only fully happen when a FinOps cultural transformation has occurred. To get to this place where cost informed data-driven decisions occur, you will have to draw upon what you have learned about FinOps and partner with your FinOps champion. This includes making sure everything is allocated appropriately (with tags, etc.) so you can have a view of the data that includes what you, the engineer, are responsible for with the right level of context. For decisions to be impactful, the data needs to be put in the path of where decisions are happening, whether this means in the design process, operating services, or monitoring services. So, talk to your FinOps team or FinOps champion if the data you need is not readily available, and get it there. 

## Enabling Engineers

To enable you to make these daily decisions about cloud spend, you need to have the right metrics presented where decisions are happening. In the same way that you can’t optimize performance without relevant metrics that illuminate user experience, you can’t optimize cost efficiency without metrics that reveal the outputs you’re getting from that spend. The goal is to bring awareness to cost metrics in the same way there is awareness around security metrics. This is where unit metrics—and the broader concept of unit economics—comes into play.

## Unit Metrics

In order to make data-driven decisions, you need to measure the things that are important to you, stakeholders, and the business. A simple definition for unit economic metrics is direct revenues or costs, associated with a particular business model, that are specifically expressed on a per-unit basis. For a customer-facing application, that unit might be a user or customer subscription; for an ecommerce platform, it might be a transaction; and for an airline, it might be cost per available seat mile.

**There is not a single unit metric that the whole organization should follow.** The FinOps practice will aim to do unit economics at multiple levels across the organization, with many different inputs and granularities. There may be high-level unit economics with metrics like cloud cost per customer, but there may also be unit economics at an application level by doing things like cost per transaction, or even do unit economics on an individual service level like compute cost per execution of a microservice.

## Calculating Unit Metrics

In every cloud unit economics calculation, there is a numerator and denominator. You’re taking something (generally an activity or output metric) and dividing it by something else (generally a portion of cloud spend) to come up with a unit metric value.

The numerator is a cloud measurement of spend that quantifies the choices made by architecture and engineering teams. The denominator is either an engineering value measurement or financial value measurement or business value measurement that gives that spend important context. The outcome of that calculation is the cloud unit economics value measurement that you’re going to use to manage some part of your business, or to give insight into what changes you could consider making.

## Unit Metrics Across the Personas

Each persona in your organization will benefit from unit metrics. 

- **Engineers** - gain an understand of cost per unit data and how decisions impact this cost per unit
- **Leaders** - gain a concept of the cost to value ratio for each area of business running in cloud
- **FinOps / Finance** - gain context to whether increases in spend are driving value or not, gain a way to represent increasing cost against the value to the business

As an engineer, your role in unit metrics, is to figure out what the unit of work for your application or suite of applications is and determine how to collect metric data from the systems you use. If you have a large blend of things, then you may have multiple units of work (some might be about supporting the customer, some might be about supporting the business). Additionally, your role includes supporting solutioning automation and identifying blocks to outputting metrics. 

Below is an example of unit metrics across an educational testing organization in the assessment industry (the provided services are designed to assess skills, aptitude, and knowledge for purposes such as educational admissions, employee recruitment and select, professional certifications, etc.). The engineering persona has found multiple unit metrics to measure. They will need to ensure these metrics are measurable across all technology systems used. Additionally, other teams are using these same metrics (especially FinOps), so you'll need to be sure your data is in an accessible location.

**Implications**

- **FinOps**: Each geographical region has isolated environments -FinOps charges back by regional cost centers
- **Engineering:** Needs to know cost per region to see trends across systems, cost per student to understand user activity of system, cost per specific cloud services to see trends of activity  
    
- **Business Owner** (selected 1 application - the scoring engine): Needs to know cost per features
- **IT Finance**: Needs to know the cost of an assessment and cost per student for RFPs and to measure against planned budget
- **C-suite**: Considering moving away from region contracts to district contracts - more direct to consume

## **Coming Back to the Iron Triangle**

Unit metrics will provide you the data needed to measure how infrastructure changes will impact costs. This means that conversations with finance become less about the technical details of the change and more about the impact they will have, freeing you up to focus on working within the unit metric-enabled financial constraints agreed upon with finance and FinOps. 

As an engineer, identifying good unit metrics creates an environment where everyone understands the costs that go into producing value. You can also focus your attention on addressing the technical details in areas that will provide the most value to the organization. It's not just about cost reporting, it's about targeting, and freeing up you, the engineer. You probably don't want people asking "why do we need all these backups" or "how come we have to use this database". We want everyone to look at the cost to operate the application, and then say "that's too high" or "this feature is not profitable" and give you the freedom to address the cost disparity.

This allows the business to make decisions that weigh the benefits of the change against the expected impact to the unit metrics, such as whether increasing the cost per active user by 2% might boost application performance by 10%, which could have positive business outcomes that make the additional investment worthwhile.

## **Desired Outcomes**

In addition to supporting trade-off conversations, when unit metrics are implemented there are several desired outcomes for the organization. 

- Quantify the cloud's role in your organization's financial performance
- Forecast profitability
- Articulate engineering contribution to gross profit margin
- Evaluate a product's business potential
- Support contribution margin, Customer Lifetime Value (LVT) or Customer Acquisition Cost (CAC)

When the cost per unit is decreasing, you will have more flexibility for increased usage (even though your bill might be higher if you used that excess savings to increase volume/output). Increased margin will add flexibility to your engineering opportunities!