# Domains & Capabilities
==Domains== describe the outcomes of FinOps practice and ==Capabilities== describe hoe to achieve them.
## Understand Usage and Cost
### Data Ingestion
Collect, transfer, store, and normalize data from various sources, with a goal of creating a complete, contextual dataset of cloud (and other technology) usage and cost data available for analysis.

Data Ingestion involves gathering, transferring, processing, transforming, and correlating various datasets to create a queryable, contextualized repository, at the appropriate level of granularity, accessibility, and completeness to support activities in all of the FinOps Capabilities across all FinOps Personas. 

The complexity of an organization's data ingestion process depends on its reliance on cloud provider tooling, third-party FinOps platforms, or the need for data from sources beyond cloud usage data. Data ingested for FinOps must include cloud cost and usage data, but may also include modified cloud billing data, carbon usage data, resource utilization or performance data, observability data, etc. Data Ingestion ensures that tags or labels created in cloud platforms are gathered and mapped to internal allocation metadata, and establishes the data sources for Reporting & Analytics(opens in a new tab).

The FinOps Open Cost & Usage Specification (FOCUS(opens in a new tab)) project aims to make billing data consistent and usable across Cloud, SaaS, and even internal billing sources, improving your understanding of your costs and allowing everyone to speak the same language to make better decisions.
### Allocation
Define strategies to assign and share cloud (and other technology) costs using accounts, tags, labels, and other metadata, creating accountability among teams and projects within an organization.

The FinOps Principle, “Everyone takes ownership for their technology usage,” is enabled by allocation. Allocation defines how costs should be apportioned to those responsible for each component of that cost, whether directly or as a shared element. 

In the context of FinOps, this involves using account structures, tags, labels, and derived metadata to identify categories to which we assign costs in a way that provides Product, Engineering, and other Personas with a transparent and complete understanding of the cost of technology resources for which they are responsible.

Allocation requires three primary strategies: 

1. **Allocation Strategy** - how costs should be mapped to the organization
    
2. **Tagging Strategy** - how cloud usage and resources will be mapped to the defined parts of the organization
    
3. **Shared Cost Strategy** - how each set of shared resources will be allocated to budgets
### Reporting and Analytics
Analyze cloud and technology consumption data and create reporting to gain insights into usage and spend patterns, identify opportunities for improvement, and support informed decision-making about cloud resources.

The Reporting & Analytics Capability provides the ability to gain insights into cloud data by creating reporting mechanisms to serve the needs of the organization’s various Persona groups. Reporting can detail, highlight, summarize, categorize, and compare data to support ad hoc reporting, showback, investigative reports, or routine reporting used by the organization. This is one of the most critical of the FinOps Capabilities, supporting almost every other Capability.

Additionally, data analysis and reporting leverages data and metadata on technology resources and resource hierarchies to create a variety of reporting mechanisms for each Persona, focusing on cost and usage data, as well as sustainability data, observability, and other related data.
### Anomaly Management
Detect, identify, alert and manage unexpected or un-forecasted cost and usage irregularities in a timely manner to lower risk in cost-effective cloud and technology operations.

Anomaly Management gives a FinOps team the ability to detect, identify, clarify, alert on, and manage unexpected cost events in a timely manner, in order to minimize impact to the business.

In the context of FinOps, anomalies are levels of spending that deviate from the normal historical or expected spend. Anomaly detection is performed by comparing current usage to past usage, which means that sudden increases in new usage or spending can trigger anomaly alerts even when they are anticipated. In such cases, teams should be prepared to see anomaly alerts and effectively manage and document them to avoid unnecessary work by other Personas.

Standard procedures for anomaly detection and analysis are essential to allow the FinOps team to react quickly when anomalies occur, often using automated, machine learning-based anomaly detection tools offered by cloud providers and third-party platforms. Managing and resolving anomalies typically involves investigation and either adjusting the environment, adjusting the expectation of the cost of the affected scope, or acknowledging and documenting the reasons for the detected anomaly.
## Quantify Business Value
### Planning and Estimating
Estimation and exploration of potential cost and value, alongside opportunities for automation, sustainability and optimization, for workloads if implemented in an organization’s cloud environment in a particular model or models.

Planning & Estimating enables organizations to estimate the future costs of a workload or system, considering the variety of services, updates, managed services, and models available in the cloud. 

Estimating can be done for any scope, from a single service change to an entire application migrating to the cloud, and is primarily supported by the Engineering Persona with input from FinOps teams, Product, Finance, or Leadership when estimates are particularly important, impactful, or complex. 

Planning & Estimating is closely related to Forecasting but focuses on exploratory ideation, producing inputs to cloud cost forecasts, and supporting FinOps Capabilities like Architecting for Cloud, Workload Optimization, or Onboarding Workloads. 
### Budgeting
The strategic and ongoing process for setting limits, monitoring, and managing cloud and other technology spending, aligned with business objectives, to ensure accountability and predictable financial outcomes for technology systems.

FinOps Budgeting establishes approved funding to support an organization's planned activities, tracks spending and value within that funding, makes transparent adjustments as needed, and ensures accountability from each budgeted cost center through consistent budgeting strategies. 

Cloud budgeting begins as part of the broader IT budgeting process and evolves as cloud use and complexity increase, requiring organizations to adopt shorter budgeting cycles with more flexibility through holdbacks and out-of-cycle adjustments.

Budgeting is closely related to Forecasting and Planning & Estimating, with budgets based on forecasts provided by teams. Budget owners are responsible for a specific scope of work, and when forecasts exceed budgets, collaboration between Personas resolves issues causing potential or actual overages.
### Unit Economics
Develop and track metrics that provide an understanding of how an organization’s cloud and technology use and management practices impact the value of the organization’s products, services, or activities.

Unit Economics bridges the gap between what an organization spends on cloud and related technology and the fundamental value that spending creates. Without understanding how to track costs to benefits received, we are missing the context that tells us whether we are spending appropriately.

Unit Economics provide the organization with important cues to be able to meet organizational goals with cloud and technology usage. They are an important method of communicating effectively between Personas and tying costs more tightly to business outcomes.
### Forecasting
Creating a model of the anticipated future cost and value of cloud and other technology systems leveraging statistical methods, historical spend patterns, planned changes, and related metrics.

Forecasting defines a model of future spending for a particular scope (a system, service, application, etc.). Forecasts are usually based on estimating, which looks at a combination of historical spending and evaluates future plans, and an understanding of how future technology infrastructure and application lifecycle changes may impact current usage.

Accurate financial forecasting depends on an organization’s other FinOps Capabilities being robust enough to provide accurate data as inputs. For example, a foundational element of this Capability is the ability to fully categorize and allocate costs.

When Finance, Engineering, and Leadership build models to forecast technology spend reliably and accurately, cost forecasting will inform investment and operational decisions to accelerate an organization’s growth. In this way, each application owner committing to its own spend forecast model, and providing those to Finance allows for not only effective budgeting, but also better management of anomalies, better decision-making related to on-premises capital spending, on value, on expected revenue, and even on environmental impacts related to sustainability.
### Benchmarking
Using efficiency metrics to evaluate cloud optimization and value between parts of the organization or against industry peers to inform decision-making and align FinOps with business objectives.

Benchmarking allows organizations to compare unit metrics and KPIs(opens in a new tab) for important aspects of cloud value and optimization both internally between different teams and externally with other organizations using cloud in similar ways.

FinOps teams should collaborate with Leadership, Product, and Engineering Personas to identify or define unit metrics or KPIs that provide insights into the organization's cloud use by being benchmarked. 

Every organization’s cloud usage will be unique. Just as there is no perfect FinOps team size or structure, benchmarking should only be one activity for assessing an organization’s cloud value and efficiency. FinOps teams must balance this Capability with other mechanisms of understanding cloud value and enabling the organization’s leadership with an understanding of the cloud investment
## Optimize Usage and Cost
### Architecting for Cloud
Designing and modernizing solutions with cost awareness and efficiency to maximize business value while achieving performance, scalability, and operational objectives.

One of the most powerful benefits of using the cloud to build systems is the ability to use a wide range of components and services to satisfy a wide range of requirements. There are many ways to build an application in the cloud. Engineering and Product teams make decisions based on the needs of the application, the knowledge and abilities of the programmers, the desired operations environment, and other factors to meet customer or stakeholder demand.

With the introduction of FinOps and broader use of cloud, Engineering and Product teams not only have the responsibility to choose services that meet the operational requirements of their systems but also the sustainability and financial viability of those systems.
### Rate Optimization

Driving cloud rate efficiency through a combination of negotiated discounts, commitment discounts (RIs, Savings Plans, Committed Use Discounts), and other pricing mechanisms to meet the organization’s operational and budgetary objectives.

Rate Optimization is the Capability that helps organizations lower the cost of resources used in the cloud by managing the rates paid for those resources. This is achieved through negotiating discounts with cloud providers, purchasing resource-based or spend-based commitment discounts, and taking advantage of usage-based discounts, special programs, or interruptible resources like Spot instances. 

A centralized FinOps team should coordinate the purchase of commitment discounts, as they are complex, have many parameters, and can be purchased in ways that allow their benefits to cover resources throughout the organization’s cloud estate.
### Licensing and SaaS
Understanding and optimizing the impact of software licenses and SaaS investments on an organization’s cloud cost structure and value by understanding vendor-specific licensing terms, use rights, and pricing options, planning for appropriate use aimed to minimize over-deployment (a compliance risk) or under-deployment (shelfware/waste), and collaborating with Finance, Procurement, and Legal teams.

In addition to IaaS (Infrastructure as a Service) cloud services, organizations often use licensed software and Software as a Service (SaaS) products, which can represent a significant area of focus for FinOps teams due to their impact on value. While billing data for SaaS or licenses may not be as granular as IaaS services, their usage is still typically variable and consumption-based. 

FinOps teams should understand how these products are being used, quantify their value, and manage their use over time. Collaboration with Procurement and ITAM (IT Asset Management) or SAM (Software Asset Management) teams is crucial to understanding purchasing methods, contractual requirements, and potential compliance risks. 

Licenses and SaaS products can be purchased through organizational agreements, bundled with cloud resources, or acquired through cloud provider marketplaces. FinOps teams must work with Procurement and ITAM to provide guidance on procurement processes and usage to Engineering and Product teams, as well as plan for adjustments to existing purchases that the organization would find valuable, considering the longer-term nature of these agreements compared to public cloud services.
### Workload Optimization
Analyze and optimize cloud resources to match specific usage patterns while ensuring that workloads operate efficiently and generate sufficient business value for their cost.

Workload Optimization is a set of practices that ensure that cloud resources are properly selected, correctly sized, only run when needed, appropriately configured, and highly utilized in order to meet all functional and non-functional requirements at the lowest cost. This work is primarily done by Engineering, using guidelines and strategies formed collaboratively with the FinOps team, Product, and other Personas.

A wide range of options exist to optimize workloads in the cloud including:

- **Waste Reduction** – removing resources that were created but are no longer being used
    
- **Workload Management** – resources should ideally be running in the cloud only when the workload is required
    
- **Scaling** – some resources have the ability to scale up or down depending on variable workload needs throughout the day/month
    
- **Rightsizing** – resources that can’t be scaled but which have more consistent low utilization may be candidates for rightsizing, reducing the size, scale, or service tier of the resource to match its workload needs
### Cloud Sustainability
Incorporating sustainability criteria and metrics into cloud optimization, to ensure environmental efficiency is balanced with financial value, and cloud optimization decisions are aligned with organizational goals.

Cloud Sustainability defines how the organization will make decisions about using cloud in ways that consider both its impact on the environment and the organization’s broader sustainability goals. Cloud Sustainability allows Engineering and Product Personas to balance environmental considerations alongside financial costs or benefits of the cloud when architecting, optimizing, and deploying workloads in the cloud.
## Manage the FinOps Practice
### FinOps Practice Operations
Driving a culture of accountability by running an effective FinOps team that empowers the FinOps practice through continuous implementation of FinOps strategy and processes.

FinOps Practice Operations involves a wide array of activities necessary to establish, operate, and mature a FinOps practice within an organization. 

Central to this is the creation of a FinOps team that works collaboratively with various stakeholders to formulate strategies, establish decision-making frameworks, and clearly delineate responsibilities related to cloud and other technology activities.
### FinOps Education and Enablement
Training, skill development, and practical activities that enable teams throughout the organization to adopt and deliver the FinOps practice.

FinOps Education & Enablement allows everyone participating in a FinOps practice to develop a common understanding of FinOps concepts, terminology, and activities. This common understanding helps to enable the collaboration that must occur across disciplines and between all parts of an organization to effectively make decisions in the context of the business value cloud and other technology provides.
### Policy and Governance
Establishing and evolving policies, controls, and governance mechanisms to ensure that cloud and technology use aligns with business objectives, complies with regulatory requirements, and optimizes resources efficiently.

Policy and governance are essential components of a successful FinOps practice, aligning cloud and technology activities with business goals and strategies, controlling resource deployment and usage to maximize ROI, and ensuring predictable and manageable costs. 

They help establish and sustain a FinOps culture by directing and inspiring people to take the right actions, monitoring outcomes, and enforcing consequences. Governance includes mechanisms to enforce policy and KPIs to measure compliance, which are shared transparently with all Personas to drive valuable behavior. Policy and governance interact with other FinOps Capabilities and operational policy and governance drivers in the organization.
### Invoicing and Showback
Developing specific reporting, cloud invoice reconciliation workflows and chargeback models, in direct collaboration with the Finance Persona with input from Product and Engineering Personas, to align cloud cost data and reporting to specific budgets and accounting requirements.

The goal of this Capability is to support Finance to allocate invoiced costs to cost centers they’ve identified, in the formats and at the timing intervals required to support accounting and finance activity required by the organization.

In addition to managing invoices, and creating chargeback reporting, this Capability must address ongoing maintenance of required data and reporting requirements over time to support maturing cloud practices and changes in accounting or finance needs. This includes providing guidance to the FinOps team on how data quality should be checked and verified, how data and reporting integrity should be maintained (e.g. some organizations will require SOC compliance or similar), what elements of cost should be included in chargeback reports (and using which cost metrics), and providing a process for situations where chargeback reporting needs to be corrected because of changes that occur after accounting period closing. The chargeback process should align to the goals of both the FinOps team and ITFM/TBM, primarily around the level of granularity for chargeback, general ledgers (cost centers) to use, and timing requirements for close activities.
### FinOps Assessment
Conducting repeatable, measurable, thoughtful analysis of the maturity of a FinOps practice in the context of the FinOps Framework for insights into strengths and areas for improvement of FinOps activities.

FinOps Assessment allows FinOps teams to measure their effectiveness, align their activities with organizational goals, and identify areas for improvement. It enables organizations to benchmark their current Capabilities and focus on the most impactful areas for creating value. 

Assessments are conducted with a representative target group and may vary based on the needs and perceptions of different groups within the organization. The goal of a FinOps Assessment is to understand the current state of maturity, define an aligned goal state, and create a pathway to achieve that goal. Assessments foster collaboration and understanding across Personas and organizational hierarchies while promoting a culture of cost awareness.
### Onboarding Workloads
Orchestrating the migration of systems into, or between, cloud environments in a way that provides transparency to cost, usage, and impact; supports operational objectives; and establishes or maintains cost effectiveness.

Moving workloads into or between cloud environments requires planning, coordination, stakeholder alignment, and an organizational strategy to determine what and how workloads and systems will be moved. 

Onboarding Workloads is typically triggered by factors such as reducing or closing down data centers, retiring capital assets, mergers or acquisitions, adopting new cloud or on-premises cloud technology, or finding the most cost-effective home for an application with a unique usage pattern. An onboarding strategy, relying on the organization's overall cloud strategy, is critical for any organization adopting public or private cloud, and a detailed migration plan is required for onboarding complex applications or workloads.
### FinOps Tools and Services
Developing criteria and methodology to effectively integrate FinOps tools and services that align to the Framework Capabilities to empower the FinOps practice.

**A FinOps Tool** refers to any of the cloud provider or third-party software packages that support any of the FinOps Capabilities. Tools range from broad FinOps platforms that support most FinOps Capabilities to targeted specialty tools that deeply support a specific activity or scope of cloud usage. 

**A FinOps Service** refers to a third-party service that delivers outcomes related to the FinOps Capabilities. These services may include training, consultancy, managed services, or even the outsourcing of parts of your FinOps practice altogether.

The tool and service strategy and the decision criteria for selecting tools will evolve over time as the organization’s needs change and mature. FinOps teams should revisit tool use regularly, particularly when major changes in cloud usage are being considered or made.
### Intersecting Disciplines
Coordinating activities with interconnected disciplines or Allied Personas (such as, ITAM, ITFM, Sustainability, Security) that manage responsibilities broader than just cloud, and which must integrate into the organizational cloud strategy by collaborating with FinOps.

This Capability supports interactions between FinOps and other IT disciplines, frameworks, or teams in an organization. Widespread use of public cloud creates new challenges for traditional IT disciplines, most of which have a broader responsibility than just cloud use. The intention for this Capability is to provide a place to capture FinOps’ interactions with these existing IT functions when they are in use by the organization.

These could include:

- IT Financial Management (ITFM)
    
- Technology Business Management (TBM)
    
- IT Asset Management (ITAM)
    
- Software Asset Management (SAM)
    
- IT Service Management (ITSM)
    
- IT Security
    
- Any other standard being used in your organization that may be impacted by cloud consumption

