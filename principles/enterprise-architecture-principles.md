---
category: Architecture Principles
expires: 2025-08-31
---
# Enterprise Architecture Principles

Enterprise Architecture Principles are general rules and guidelines that inform and support decisions in how DfE should deliver solutions to align with its vision and objectives. They are intended to be enduring and seldom amended. They reflect a level of consensus across the organisation (our 'enterprise') and embody the spirit and thinking of the enterprise architecture.

Discovery, user research and requirements gathering provide user needs and wants which inform what a solution does; principles provide guidance on how solutions should be architected to meet those needs.

These principles should be applied alongside the UK Government [Service Standard](https://www.gov.uk/service-manual/service-standard) and [Technology Code of Practice](https://www.gov.uk/government/publications/technology-code-of-practice/technology-code-of-practice).

---

# The Principles

1.	[Business Alignment](#1align-with-business-objectives)
2.	[Standardisation](#2standardisation)
3.	[Flexibility and Adaptability](3flexibility-and-adaptability)
4.	[Security and Compliance](4security-and-compliance)
5.	[Cloud First](5cloud-first---rent-before-buy-before-build).
6.	[Data Integrity and Quality](6data-integrity-and-quality)
7.	[Reuse and Modularity](7reuse-and-modularity)
8.	[Design for Operation](8design-for-operation)
9.	["Good Enough” Solutions](9good-enough-solutions)

---

# 1.	Align with business objectives
## 1.1.	Description
Align and prioritise digital, data and technology (DDT) strategies and deliveries with business 
goals and objectives, to maximise taxpayer value.
## 1.2.	Rationale
*	Changes in ministerial priorities cause volatility in the goals and objectives of the 
department. 
*	Ensuring delivery aligns with departmental goals and objectives improves efficiency, 
with better resource allocation and decision-making. 
## 1.3.	Implications
*	To maximise taxpayer value, review deliveries as business and ministerial goals change, 
ensuring appropriate investment of effort and money.
*	Ensure value by linking delivery metrics to business objectives, which also facilitates 
rapid review of relevance when goals and objectives change.
*	Work may be deprioritised or stopped as business goals and objectives change. 
*	Invest in functionality and delivery that has long-term stability through changing 
government policies and priorities.
*	User needs may not align with DFE business objectives, therefore cost and value of 
delivering these capabilities should be weighed against the impact to achieving 
departmental objectives

---

# 2.	Standardisation
## 2.1.	Description
Adherence to DFE standards and patterns promote consistency, simplify the landscape, and 
minimise technical debt.

## 2.2.	Rationale
*	Use of consistent technologies and platforms facilitates interoperability, reduces 
complexity, and simplifies maintenance.
*	Quicker onboarding of suppliers and reduced time and cost spent on evaluating 
technology options.
*	It becomes easier to reallocate resources between deliveries to optimise deliveries and 
accommodate changing priorities. 
*	Consistent technology choices reduce technical debt and proliferation of technology 
within the department.
*	Streamlined processes, easier integration, and cost savings through economies of 
scale.

## 2.3.	Implications
*	Productivity of individuals and teams may reduce as they transition to standard tools 
and platforms; expect some retraining requirements.
*	Pragmatism means one tool or platform may not be desirable or achievable, need to link 
to use cases and allow exceptions for unusual scenarios.
*	Standards need developing and managing across all areas of DDT.
*	Standards need processes and governance to adapt to changing needs and modern 
technologies. 
*	Need ability to experiment with modern technologies to evaluate usefulness.

---

# 3.	Flexibility and Adaptability
## 3.1.	Description 
Design systems that can adapt to changing business needs and technological advancements.

## 3.2.	Rationale 
*	Ministerial priorities will change. Business environments evolve rapidly; agility is 
essential to serve users effectively. 
*	Reduced risk of obsolescence, quicker response to market changes.

## 3.3.	Implications 
*	Continuous development is expensive, design solutions to allow for predictable change 
without redevelopment. 
*	Predict the types of change that will affect your solution area and accommodate these 
in the design through configuration or replaceable/expandable modules.
*	Delivery of flexible and adaptable solutions will be more complex and costly initially, 
offset by reduced future cost of change.
*	Change may not happen; do not cover every eventuality, only consider changes that 
could be expected within the lifecycle of a product. 

 ---

# 4.	Security and Compliance
## 4.1.	Description 
Prioritise security measures and regulatory compliance in architectural decisions.

## 4.2.	Rationale 
*	Good security practices protect data, maintains trust, and avoids reputational damage, 
impact to customers and legal penalties.
*	Understanding threats, vulnerabilities and applying mitigations at design stage reduces 
cost of delivering secure services and prevents vulnerabilities risking DFE data and 
services.

## 4.3.	Implications 
*	Conduct threat modelling early in a service lifecycle and review as threats and the 
service evolve. 
*	Apply threat modelling to all components and flows in your solution from both external 
and internal threat actors and apply appropriate mitigations.
*	Threat mitigations should be prioritised in backlogs to prevent exploitation of 
vulnerabilities.
*	A system is only as secure as its weakest link, therefore all components, modules and 
flows should be protected regardless of the sensitivity of data held by that solution. 
*	Exploitation of weak points can provide a stepping stone into other solutions, platforms, 
and data, therefore even if your solution is considered lower risk, protections are 
required to prevent your system becoming a back door into sensitive data elsewhere in 
the organisation.

---

# 5.	Cloud First - Rent before buy before build
## 5.1.	Description 
Do not build what can easily bought off-the-shelf. Prioritise cloud-based solutions over on-
premises alternatives.

## 5.2.	Rationale 
*	Commercial-off-the-shelf (COTS) solutions include cost of development, operation, and 
best practice their costs and share these between all clients therefore Total Cost of 
ownership (TCO) is cheaper for “utility” functionality. 
*	Leverage scalability, cost-effectiveness, and agility of cloud services.

## 5.3.	Implications 
*	Conduct an options appraisal before choosing delivery approach. 
*	Evaluate COTS solutions against “good enough” as they are unlikely to meet all 
requirements; they may need façades, configuration, or a hybrid approach to meet user 
needs e.g. If a COTS solution delivers 80% of user needs, consider wrapping or 
extending the COTS solution for the remaining 20%, rather than building 100% bespoke.
*	Avoid customisation of COTs solutions to deliver bespoke functionality, where required 
use configuration and integration to tailor the solution to user needs. Adapt business 
processes to align with COTS where possible. 
*	Develop an exit plan before adopting COTS to prevent vendor lock-in. 
*	Evaluate TCO between COTS and bespoke, including hosting, delivery resource, 
support, and platform costs for the lifetime of the product, during options appraisal.
*	Prioritise Software-as-a-Service (SaaS) solutions, over Platform-as-a-Service (PaaS) 
over Infrastructure-as-a-Service (IaaS), over on-premise, when evaluating solution 
hosting options.

---

# 6.	Data Integrity and Quality
## 6.1.	Description 
Ensure accurate, consistent, and reliable data across DFE IT Landscape. Use master data sources and, when mastering data, make it available to other services through interfaces that ensure data consistency, integrity and quality. 

## 6.2.	Rationale 
*	Reliable data drives informed decision-making and operational efficiency. 
*	Duplication or poor data management practices reduce user trust, introduce errors, 
discrepancies and data quality issues whilst increasing cost and effort of data collation 
and analysis. 
*	By creating and using trusted shared data sources, services can provide consistent 
data, improving user experience and trust and reduce data engineering costs in 
preparing data for analysis.

## 6.3.	Implications 
*	Use authoritative data sources without creating copies. 
*	Authoritative data sources must have availability and scalability to meet service 
demands with appropriate support and service levels.
*	Embed data management and governance practices in the organisation and for both 
operational and analytical data.

---

# 7.	Reuse and Modularity
## 7.1.	Description
Solve problems once, encourage creation and reuse of components, services and patterns.

## 7.2.	Rationale 
*	Delivering services and functionality is expensive, by avoiding reinventing the wheel we 
can streamline development efforts, reduce duplication and costs. 
*	By decomposing services into small reusable components teams can consume these 
rather than building functionality from scratch.
*	Services can be delivered by assembling existing components more quickly, cheaply, 
and consistently than duplicating functionality.
*	Capabilities cross organisational and service boundaries therefore reuse can break 
down the silos that naturally form around portfolio centred teams and create a more 
consistent user experience. 
*	Modularity allows rearrangement of components and functionality when policy or 
organisational goals or objectives change. 
*	Updates to shared components automatically apply to all dependent services; when 
making changes only the component changes and therefore can reduce testing 
required.
*	Measurement of use of components allows better understanding of user journeys to 
inform policy and delivery decisions.

## 7.3.	Implications 
*	Interdependencies between services and teams increase complexity and will slow initial 
deliveries.
*	Assume that someone will need to reuse any new capabilities you deliver, look for 
similarities rather than differences, only build what does not exist already, and make it 
reusable. Where there are differences consider encapsulation or abstraction to extend 
the base functionality; and make that a service.
*	Changes to components need to be non-breaking to avoid failures in dependant 
systems.
*	Make services small and re-useable, breaking functionality into separate modules or 
components with integration capabilities. 
*	Facilitate synchronous and/or asynchronous integrations as appropriate. 
*	Separate front-end functionality from back-end components, back-ends should not 
depend on front end validation or other functionality to function correctly. 
*	Design and scale each component for availability and re-use; Consider “circuit 
breakers” for latency and non-responsiveness of components but avoid duplication as 
mitigation.
*	Components need to support all users equally. 
*	Need capability teams to discover existing components, services and patterns and the 
functionality they provide?

---

# 8.	Design for Operation
## 8.1.	Description 
Architect systems with operational efficiency, reliability and sustainability in mind.

## 8.2.	Rationale 
*	Smooth operations reduce downtime, enhance reliability and availability. 
*	Designing for efficient operations, with appropriate availability and scalability without 
manual intervention drives reduced TCO.
*	The majority of costs for any solution occur post-delivery and therefore architects 
should avoid short-term decisions to minimise delivery costs or accelerate delivery 
timescales that adversely impact the organisation or stakeholders long-term.

## 8.3.	Implications 
*	Design systems with appropriate resilience and scalability to meet service needs and 
those of any dependent services, where possible automate these to avoid service 
impacts in the event of sudden demand or failures.
*	Services may need different levels of availability and scalability for each module or 
component of their service; overall service availability and scalability is only as good as 
its weakest link. Plan and test for DR/BC scenarios and peak loads to ensure service 
designs are appropriate.
*	Automation and integration of solution operations to common CMDB, service logging 
and monitoring platforms promotes easier maintenance, proactive monitoring, and 
better support with reduced resource requirements. 
*	All projects delivering solutions to replace existing services or components need to 
include decommissioning of the old system in the project activity and costs to avoid 
technical debt.
*	Automate delivery pipelines to update CMDB/service catalog to ensure information is 
always up to date during delivery phase.
*	Evaluate the long-term viability of suppliers and products to prevent tech-debt or risk of 
supplier failure.
*	Architectural decisions need to factor the expected life cycle of the solution and its 
impact on stakeholders, the environment, and total cost of ownership. 
*	Decisions need to prioritise prevention of technical debt, minimise rework, ensure 
future scalability (up and down), and optimise operational resource and cost demands. 
*	Include full lifecycle people and technical resource costs in TCO comparisons when 
evaluating options.

---

# 9.	“Good Enough” Solutions
## 9.1.	Description 
Recognize that perfection is not always necessary. Strive for solutions that meet essential 
requirements without unnecessary features. Prioritise value over perfection, especially in agile 
and iterative contexts.
## 9.2.	Rationale 
*	Balancing pragmatism with quality allows for faster delivery, adaptability and maximises 
taxpayer value whilst Minimising delivery costs and allowing resources to pivot to other 
deliveries. Pareto rule – 20% of functionality delivers 80% of the value.
## 9.3.	Implications 
*	Architecture needs to reflect the emergent nature of agile delivery and therefore do “just 
enough” architecture to enable delivery; this means longer term architecture should still 
be done, but at an appropriate level to adapt as detail emerges through delivery.
*	Avoid “gilding the lily” or over-engineering, focus on critical features, and iterate based 
on feedback. Measure VFM of each feature including costs of delivery resources over 
realistic lifetime of the product before adding to backlog. Stop when the service reaches 
“good enough”. 
*	Evaluate cost saving of COTS options with good-enough functionality against bespoke 
delivery.
*	Ensure compliance with legislative, accessibility and security standards.
*	Have a “definition of done”, check regularly whether this criteria has been met 
