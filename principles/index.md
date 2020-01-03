---
category: Architecture Principles
expires: 2020-01-01
---

# Enterprise Architecture Principles

Principles are general rules and guidelines, intended to be enduring and seldom amended, that inform and support the way in which the DfE fulfils its vision and principles. They reflect a level of consensus across the enterprise and embody the spirit and thinking of the enterprise architecture.

Requirements gathering provide user needs and wants, principles provide the guidance to meet those requirements.

## 1. Re-use standardised approved services and components

__Why?__

Duplication of services or components adds cost and complexity.

__How?__
- When re-using components and services, projects are likely to need to assemble several components / services to meet end-to-end requirements and not just look for single solutions
- Where no approved service or component exists, any new service or component should be designed to maximise re-usability
- Services or components should be delivered at the smallest possible granularity to facilitate re-use

__Relates to__

- TCoP8: Share, reuse and collaborate
- SS2: Solve a whole problem for users.
- SS13: Use and contribute to open standards, common components and patterns

## 2. Align technology choices with cross government strategies and services

__Why?__

x

__How?__
- x

__Relates to__

- x

Number | Principle | Rationale (reason for adoption) | Implication (what are the consequences of conforming to this principle) | GDS service standard (SS) / Technology Code of Practice (TCoP) alignment
- | - | - | - | -
1 | Re-use standardised approved services/ components | Duplication of services or components adds cost and complexity. | * When re-using components and services, projects are likely to need to assemble several components / services to meet end-to-end requirements and not just look for single solutions. *	 Where no approved service or component exists , any new service or component should be designed to maximise reusability.	 * Services or components should be delivered at the smallest possible granularity to facilitate re-use | * TCoP8: Share, reuse and collaborate. * SS2: Solve a whole problem for users.* SS13: Use and contribute to open standards, common components and patterns
2 | Align technology choices with cross government strategies and services| Components and services should be aligned with government strategies to increase reusability, minimise cost and improve consistency of user experience across government services. Cross government components include Gov.UK Notify, Gov.UK Verify, Gov.UK Pay etc | Projects delivering new products or services should assess alignment with cross government strategies and deliver re-useable components and services which can be used at cross-government level | SS3: Provide a joined up experience across all channels
3 | Technology decisions and project choices must be linked to DfE goals and drivers | Technology investment should only be made where it demonstrably contributes to DfE goals or drivers | * All projects should have a business case with measurable business outcomes aligned to DfE Goals and drivers. * All projects shall assign a person accountable for measurement, reporting and realisation of stated business benefits | SS10: Define what success looks like and publish performance data
4 | Total Cost of Ownership must be evaluated | Expenditure of public money should always look to deliver the best value for the taxpayer. Ongoing support and maintenance of solutions form a major part of the total costs and therefore should inform technology decisions. Ongoing support and maintenance of solutions form a major part of the total costs and therefore should inform technology decisions | * All projects above the agreed set threshold, must be supported by an evidenced business case, ensuring that overall solution costs have been considered for value for money. * For all projects the Architecture partner must asses the total cost of ownership and challenge where appropriate * Where duplicate service or component is proposed TCO should include costs of running both/all duplicated services * Investment must justified by supporting evidence. * Design must consider long term costs and support of any solution delivered | SS10: Define what success looks like and publish performance data
5 | Data is a shared asset | We are striving to be a data-driven department: Data is the golden thread that supports seamless, user-centric user journeys.  Data enables evidence based decisions to be made, supports management and governance of our business activities, is used to hold us to account for delivery and allows us to assess the effectiveness of our Departmental policies. | * Data must be sharable – solutions should adhere to Departmental Data Standards, working with DfE Data Governance team to extend those standards if necessary. * Data must be shared – services should provide methods of sharing data with other services to support other user journeys, and with the Enterprise Data & Analysis Platform to support reporting, analysis and Data Science. * Data must be protected – services must take care during both development and operational phases to adequately secure live data, including but not limited to data containing Personally Identifiable Information. * Architects must follow the Departmental Data Protection policies held by the DfE Data Governance team to ensure they are protecting our shared assets appropriately.  | TCoP10: Make better use of data
6 | Consider buy before build | Provides for economies of scale, should reduce risk and timescales | * Requirements may need to be prioritised or forfeited to avoid bespoke solutions * Using multiple integrated solutions may be necessary to satisfy complex user needs * Configuration is likely to be necessary to use COTS, customisation should be avoided | SS11: Choose the right tools and technology
7 | Design for accessibility | Provides an equal playing field for all users | * Systems must adhere to current government accessibility regulations.	* Seek input from Accessibility Advisers on how designs might need amending to improve accessibility * Include accessibility testing as part of any project delivery |TCoP2: Make things accessible and inclusive * SS4: Make the service simple to use * SS5: Make sure everyone can use the service
8 | Deliver a secure service | The department’s information assets must be protected to ensure that they are not inadvertently exposed to an unintended audience. | * Early engagement with the Chief Information Security Officer (CISO) division will ensure that risk assessments are completed and appropriate security controls are designed into solutions before development has begun. * Security controls must be proportionate to ensure that it is still possible for authorised users to access and share data seamlessly. | * TCoP6: Make things secure * SS9: Create a secure service which protects users' privacy.
9 | Deliver cloud-only solutions | The scale of public cloud services enables the delivery of highly scalable, cost effective, secure services. Consumption based billing and rapid provisioning supports the Government ICT strategy. A service can be configured and built using a SaaS product, without bespoke customisation and  vendor lock in. | * Software as a Service (SaaS) before Platform as a Service (PaaS) before Infrastructure as a Service (IaaS) * Check hosting arrangements and data sensitivity when selecting cloud solutions * Design exit strategy before entering cloud agreements * Design solutions to take advantage of cloud features e.g. elastic scaling, spin down | TCoP5: Use cloud first
10 | Design for interoperability | Interoperability enables sharing of capabilities and data between systems |* Service Oriented and Microservice architectures maximise interoperability and re-use * Interfaces should be discoverable and self-describing  or documented. * Interoperability can affect the demands on solutions, therefore designs may need to be scalable to cope with other usage | TCoP9: Integrate and adapt technology
11 | Open standards must be considered | Avoidance of vendor lock-in. Lays the foundation for delivering interoperability. Open standards facilitate interoperability and data exchange among different products or services. | Where open standards do not exist, create one or find the best fit with least lock in  | * TCoP4: Make use of open standards * SS13: Use and contribute to open standards, common components and patterns
12 | Design for portability | Avoidance of vendor lock-in. Moving to a new platform is simpler and requires less engineering |* Design must be platform agnostic. * Minimise use platform specific features * Will require an exit strategy |
13 | Solutions must be loosely coupled | Loosely coupled components can be replaced with alternative implementations that provide the same services. Components in a loosely coupled system are less constrained to the same platform, language, operating system, or build environment. | * Projects must ensure any additional coordination protocols needed are in place. * Projects must ensure consistent data synchronisation with DfE Data guidance | TCoP9: Integrate and adapt technology
14 | Minimise technical debt | Replacing or superseding a component or service without removing existing components or services increases technical debt | <Li>Any project delivering a technology component or service designed to supersede or replace an existing component or service must remove the existing service as part of that project</li> <li>Project budgets need to include cost of decommissioning existing solutions or include total cost  of both systems in the business case. | SS2. Solve the whole problem for a users
