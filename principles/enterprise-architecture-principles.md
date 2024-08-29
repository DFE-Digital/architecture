---
category: Architecture Principles
expires: 2025-08-31
---
# Enterprise Architecture Principles

Enterprise Architecture principles are general rules and guidelines that inform and support decisions in how DfE should deliver services, to align with its vision and objectives. 

They are intended to be enduring and seldom amended. They reflect a level of consensus across the organisation (our 'enterprise') and embody the spirit and thinking of the enterprise architecture.

Discovery, user research and requirements gathering provide user needs (and wants), which inform what a service does. Principles provide guidance on how services should be architected to meet those needs.

These principles should be applied alongside the UK Government [Service Standard](https://www.gov.uk/service-manual/service-standard) and [Technology Code of Practice](https://www.gov.uk/guidance/the-technology-code-of-practice).

---

1.	[Business alignment](#1-align-with-business-objectives)
2.	[Standardisation](#2-standardisation)
3.	[Flexibility and adaptability](#3-flexibility-and-adaptability)
4.	[Security and compliance](#4-security-and-compliance)
5.	[Cloud First](#5-cloud-first---rent-before-buy-before-build)
6.	[Data integrity and quality](#6-data-integrity-and-quality)
7.	[Reuse and modularity](#7-reuse-and-modularity)
8.	[Design for operation](#8-design-for-operation)
9.	['Good enough' services](#9-good-enough-services)

---

## 1. Align with business objectives

### 1.1.	Description
Align and prioritise digital, data and technology (DDT) strategies and delivery with DfE's business 
goals and objectives, to maximise taxpayer value

### 1.2.	Rationale
*	Changes in ministerial priorities cause volatility in the goals and objectives of the 
department
*	Ensuring delivery aligns with departmental goals and objectives improves efficiency, 
with better resource allocation and decision-making

### 1.3.	Implications
*	To maximise taxpayer value, review deliveries as business and ministerial goals change, 
ensuring appropriate investment of effort and money
*	Ensure value by linking delivery metrics to business objectives, which also facilitates 
rapid review of relevance when goals and objectives change
*	Work may be deprioritised or stopped as business goals and objectives change. 
*	Invest in functionality and delivery that has long-term stability through changing 
government policies and priorities
*	User needs may not align with DfE business objectives, therefore the cost and value of 
delivering the capabilities should be weighed-up against the impact to achieving 
departmental objectives

---

## 2. Standardisation

### 2.1.	Description
Adhere to DfE standards and patterns, to promote consistency, simplify the landscape and 
minimise technical debt

### 2.2.	Rationale
*	Use of consistent technologies and platforms facilitates interoperability, reduces 
complexity and simplifies maintenance
*	Quicker onboarding of suppliers, with reduced time and cost on evaluating 
technology options
*	It becomes easier to reallocate resources between deliveries, to optimise deliveries and 
accommodate changing priorities
*	Consistent technology choices reduce technical debt and proliferation of technology 
within the department
*	Streamlined processes, easier integration and cost savings through economies of 
scale

### 2.3.	Implications
*	Productivity of individuals and teams may reduce as they transition to standard tools 
and platforms - expect some retraining requirements
*	Pragmatism means one tool or platform may not be desirable or achievable - need to link 
to use cases and allow exceptions for unusual scenarios
*	Standards need developing and managing across all areas of DDT
*	Standards need processes and governance to adapt to changing needs and modern 
technologies
*	Need the flexibility to experiment with modern technologies to evaluate usefulness

---

## 3. Flexibility and adaptability

### 3.1.	Description 
Design services that can adapt to changing business needs and technological advancements

### 3.2.	Rationale 
*	Ministerial priorities will change. Business environments evolve rapidly - agility is 
essential to serve users effectively.
*	Reduced risk of obsolescence, quicker response to market changes

### 3.3.	Implications 
*	Continuous development is expensive - design services to allow for predictable change 
without redevelopment
*	Predict the types of change that will affect your service area and accommodate these 
in the design, through configuration or replaceable/expandable modules
*	Delivery of flexible and adaptable services will be more complex and costly initially, 
offset by reduced future cost of change
*	Change may not happen - do not cover every eventuality, only consider changes that 
could be expected within the lifecycle of a service/product

 ---

## 4. Security and compliance

### 4.1.	Description 
Prioritise security measures and regulatory compliance in architecture decisions

### 4.2.	Rationale 
*	Good security practices protect data, maintain trust and avoids reputational damage, 
impact to customers and legal penalties
*	Understanding threats, vulnerabilities and applying mitigations at the design stage reduces 
the cost of delivering secure services and prevents vulnerabilities risking DfE data and 
services

### 4.3.	Implications 
*	Conduct threat modelling early in a service lifecycle and review, as threats and the 
service evolve
*	Apply threat modelling to all components and flows in your service, from both external 
and internal threat actors, and apply appropriate mitigations
*	Threat mitigations should be prioritised in backlogs to prevent exploitation of 
vulnerabilities
*	A system is only as secure as its weakest link - all components, modules and 
flows should be protected regardless of the sensitivity of data held by that service 
*	Exploitation of weak points can provide a stepping stone into other services, platforms, 
and data - even if your service is considered lower risk, protections are 
required to prevent your system becoming a 'back door' into sensitive data elsewhere in 
the organisation

---

## 5. Cloud First - rent, before buy, before build

### 5.1.	Description 
Do not build what can easily be bought off-the-shelf. Prioritise cloud-based services over on-premises alternatives.

### 5.2.	Rationale 
*	Commercial-off-the-shelf (COTS) services include the cost of development, operation and 
best practice in their costs, and share these between all clients. Total Cost of 
Ownership (TCO) is cheaper for 'utility' functionality.
*	Leverage scalability, cost-effectiveness and agility of cloud services

### 5.3.	Implications 
*	Conduct an options appraisal before choosing a delivery approach 
*	Evaluate COTS solutions against what's “good enough”, as they are unlikely to meet all 
requirements - they may need façades, configuration or a hybrid approach to meet user 
needs. For example, if a COTS solution delivers 80% of user needs, consider wrapping or 
extending the COTS solution for the remaining 20%, rather than building 100% bespoke.
*	Avoid customisation of COTS solutions to deliver bespoke functionality. Where required, 
use configuration and integration to tailor the solution to user needs. Adapt business 
processes to align with COTS where possible.
*	Develop an exit strategy before adopting COTS, to prevent vendor lock-in 
*	Evaluate TCO between COTS and bespoke options during options appraisal. This should include
 hosting, platform, delivery resource and support costs, for the lifetime of the product.
*	Prioritise Software-as-a-Service (SaaS) services, over Platform-as-a-Service (PaaS), 
over Infrastructure-as-a-Service (IaaS), over on-premises options, when evaluating service 
hosting options

---

## 6. Data integrity and quality

### 6.1.	Description 
Ensure accurate, consistent and reliable data across DfE. Use master data sources and, when mastering data, make it available to other services through interfaces

### 6.2.	Rationale 
*	Reliable data drives informed decision-making and operational efficiency
*	Duplication or poor data management practices reduces user trust, introduces errors, 
discrepancies and data quality issues, whilst increasing the cost and effort of data collation 
and analysis
*	By creating and using trusted shared data sources, services can provide consistent 
data, improve user experience and trust, and reduce data engineering costs, in 
preparing data for analysis

### 6.3.	Implications 
*	Use authoritative data sources without creating copies, to ensure data consistency, integrity and quality
*	Authoritative data sources must have availability and scalability to meet service 
demands, with appropriate support and service levels
*	Embed data management and governance practices in the organisation for both 
operational and analytical data

---

## 7. Reuse and modularity

### 7.1.	Description
Solve problems once, encouraging the creation and reuse of components, services and patterns

### 7.2.	Rationale 
*	Delivering services and functionality is expensive - by avoiding reinventing the wheel, we 
can streamline development efforts, reduce duplication and costs
*	By decomposing services into small reusable components, teams can consume these 
rather than building functionality from scratch
*	Services can be delivered by assembling existing components quicker, cheaper 
and more consistently than duplicating functionality
*	Capabilities cross organisational and service boundaries - reuse can break 
down the silos that naturally form around portfolio-centred teams and create a more 
consistent user experience
*	Modularity allows rearrangement of components and functionality when policy or 
organisational goals or objectives change
*	Updates to shared components automatically apply to all dependent services - when 
making changes, only the component changes which reduces the testing required
*	Measuring the of use of components allows better understanding of user journeys, to 
inform policy and delivery decisions

### 7.3.	Implications 
*	Interdependencies between services and teams increases complexity and will slow delivery
initially 
*	Assume that someone will need to reuse any new capabilities you deliver - look for 
similarities rather than differences, only build what does not exist already, and make it 
reusable. Where there are differences consider encapsulation or abstraction to extend 
the base functionality, and make that a service.
*	Changes to components need to be non-breaking to avoid failures in dependant 
systems
*	Make services small and re-useable, breaking functionality into separate modules or 
components with integration capabilities 
*	Facilitate synchronous and/or asynchronous integrations, as appropriate 
*	Separate front-end functionality from back-end components - back-ends should not 
depend on front-end validation (or other functionality) to work correctly 
*	Design and scale each component for availability and re-use - consider 'circuit 
breakers' for latency and non-responsiveness of components but avoid duplication as 
mitigation
*	Components need to support all users equitably
*	Requires teams to be able to discover existing components, services and patterns, and the 
functionality they provide

---

## 8. Design for operation

### 8.1.	Description 
Architect systems and services with operational efficiency, reliability and sustainability in mind

### 8.2.	Rationale 
*	Smooth service operations reduce downtime, enhance reliability and availability
*	Designing for efficient operations, with appropriate availability and scalability without 
manual intervention, drives reduced TCO
*	The majority of costs for any service occur post-delivery - avoid short-term decisions to 
minimise delivery costs, or accelerate delivery timescales that adversely impact the 
organisation or users long-term.

### 8.3.	Implications 
*	Design systems with appropriate resilience and scalability to meet service needs, and 
those of any dependent services. Where possible, automate these to avoid service 
impacts in the event of sudden demand or failures.
*	Services may need different levels of availability and scalability for each module or 
component. Overall service availability and scalability is only as good as 
its weakest link. Plan and test for Disaster Recovery and Business Continuity scenarios, 
as well as peak loads, to ensure service designs are appropriate.
*	Automation and integration of service operations to a common Configuration Management 
Database (CMDB), logging and monitoring platforms promotes easier maintenance, proactive 
monitoring and better support, with reduced resource requirements. 
*	All projects delivering services that replace existing services or components must 
include decommissioning of the old service(s) or component(s) in the project activity and costs,
 to actively reduce technical debt
*	Automate delivery pipelines to update CMDB / Service Catalogue, to ensure information is 
always up to date during delivery phases
*	Evaluate the long-term viability of suppliers and products, to prevent technical debt or risk of 
supplier failure
*	Architecture decisions need to factor the expected lifecycle of the service and its 
impact on stakeholders, the environment and TCO
*	Decisions need to prioritise prevention of technical debt, minimise rework, ensure 
future scalability (up and down) and optimise operational resource and cost demands
*	Include full-lifecycle people and technical resource costs in TCO comparisons when 
evaluating options

---

## 9. 'Good enough' services

### 9.1.	Description 
Recognise that perfection is not always necessary. Strive for services that meet essential 
requirements without unnecessary features. Prioritise value over perfection, especially in agile 
and iterative contexts.

### 9.2.	Rationale 
* Balancing pragmatism with quality allows for faster delivery, adaptability and maximises 
taxpayer value, whilst minimising delivery costs and allowing people to pivot to other 
delivery
* Pareto rule – 20% of functionality delivers 80% of the value

### 9.3.	Implications 
*	Architecture needs to reflect the emergent nature of agile delivery and therefore do 'just 
enough' architecture to enable delivery. This means longer term architecture should still 
be done, but at an appropriate level to adapt, as detail emerges through delivery.
*	Avoid “gilding the lily” or over-engineering - focus on critical features and iterate based 
on feedback. Measure the value for money of each feature, including cost of delivery resources over 
a realistic lifetime of the service before adding to backlog. Stop when the service reaches 
'good enough'.
*	Evaluate the cost saving of COTS options with 'good-enough' functionality against bespoke 
delivery
*	Ensure compliance with legislative, accessibility and security standards
*	Have a 'definition of done' - check regularly whether this criteria has been met
