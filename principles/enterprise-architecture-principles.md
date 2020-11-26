---
category: Architecture Principles
expires: 2021-01-01
---

# Enterprise Architecture Principles

Principles are general rules and guidelines, intended to be enduring and seldom amended, that inform and support the way in which the DfE fulfils its vision and principles. They reflect a level of consensus across the enterprise and embody the spirit and thinking of the enterprise architecture.

Requirements gathering provide user needs and wants, principles provide the guidance to meet those needs.

Throughout these principles, we refer to specific points of the UK Government [Service Standard](https://www.gov.uk/service-manual/service-standard) and [Technology Code of Practice](https://www.gov.uk/government/publications/technology-code-of-practice/technology-code-of-practice), that underpin use of these principles.

## 1. Re-use services and components

__Why?__

Duplication of services or components adds cost and complexity.

__How?__
- When re-using components and services, projects are likely to need to assemble several components / products to meet end-to-end requirements and not just look for single solutions
- Where no approved service or component exists, any new service or component should be designed to maximise re-usability
- Services or components should be delivered at the smallest possible granularity to facilitate re-use

__Relates to__

- [TCoP8](https://www.gov.uk/government/publications/technology-code-of-practice/technology-code-of-practice#share-reuse-and-collaborate): Share, reuse and collaborate
- [SS2](https://www.gov.uk/service-manual/service-standard/point-2-solve-a-whole-problem): Solve a whole problem for users.
- [SS13](https://www.gov.uk/service-manual/service-standard/point-13-use-common-standards-components-patterns): Use and contribute to open standards, common components and patterns

## 2. Align technology choices with cross-Government strategy

__Why?__

Components and services should be aligned with government strategies to increase reusability, minimise cost and improve consistency of user experience across government services. Cross government components include Gov.UK Notify, Gov.UK Verify, Gov.UK Pay - read more about [Government as a Platform](https://gds.blog.gov.uk/category/government-as-a-platform/) on the GDS blog.

__How?__

Projects delivering new products or services should assess alignment with cross government strategies and deliver re-useable components and services which can be used at cross-government level

__Relates to__

[SS3](https://www.gov.uk/service-manual/service-standard/point-3-join-up-across-channels): Provide a joined up experience across all channels

## 3. Link technology decisions to DfE goals

__Why?__

Technology investment should only be made where it demonstrably contributes to DfE goals or drivers

__How?__
- All projects should have a business case with measurable business outcomes aligned to DfE Goals and drivers.
- All projects should assign a person accountable for measurement, reporting and realisation of stated business benefits

__Relates to__

- [SS10](https://www.gov.uk/service-manual/service-standard/point-10-define-success-publish-performance-data): Define what success looks like and publish performance data

## 4. Evaluate Total Cost of Ownership

__Why?__

- Expenditure of public money should always look to deliver the best value for the taxpayer
- Ongoing support and maintenance of solutions form a major part of the total costs and therefore should inform technology decisions

__How?__
-  All projects above the agreed set threshold, must be supported by an evidenced business case, ensuring that overall solution costs have been considered for value for money.
-  For all projects the Architecture partner must asses the total cost of ownership and challenge where appropriate
-  Where duplicate service or component is proposed TCO should include costs of running both/all duplicated services
-  Investment must justified by supporting evidence.
-  Design must consider long term costs and support of any solution delivered

__Relates to__

- [SS10](https://www.gov.uk/service-manual/service-standard/point-10-define-success-publish-performance-data): Define what success looks like and publish performance data

## 5. Data is a shared asset

__Why?__

We are striving to be a data-driven department: data is the golden thread that supports seamless, user-centric user journeys.  Data enables evidence based decisions to be made, supports management and governance of our business activities, is used to hold us to account for delivery and allows us to assess the effectiveness of our Departmental policies.

Read more about our [Enterprise Data Architecure principles](/enterprise-data-architecture-principles)

__How?__

-  Data must be sharable – solutions should adhere to Departmental Data Standards, working with DfE Data Governance team to extend those standards if necessary.
-  Data must be shared – services should provide methods of sharing data with other services to support other user journeys, and with the Enterprise Data & Analysis Platform to support reporting, analysis and Data Science.
-  Data must be protected – services must take care during both development and operational phases to adequately secure live data, including but not limited to data containing Personally Identifiable Information. Architects must follow the Departmental Data Protection policies held by the DfE Data Governance team to ensure they are protecting our shared assets appropriately.

__Relates to__

- [TCoP10](https://www.gov.uk/government/publications/technology-code-of-practice/technology-code-of-practice#make-better-use-of-data): Make better use of data


## 7. Deliver a secure service  

__Why?__

The department’s information assets must be protected to ensure that they are not inadvertently exposed to an unintended audience.

__How?__
-   Early engagement with the Chief Information Security Officer (CISO) division will ensure that risk assessments are completed and appropriate security controls are designed into solutions before development has begun
-  Security controls must be proportionate to ensure that it is still possible for authorised users to access and share data seamlessly

__Relates to__

- [TCoP6](https://www.gov.uk/government/publications/technology-code-of-practice/technology-code-of-practice#make-things-secure): Make things secure
- [SS9](https://www.gov.uk/service-manual/service-standard/point-9-create-a-secure-service): Create a secure service which protects users' privacy

## 8. Deliver cloud-native solutions

__Why?__

- The scale of public cloud services enables the delivery of highly scalable, cost effective, secure services. Consumption based billing and rapid provisioning supports the Government ICT strategy.
- A service can be configured and built using a SaaS product, without bespoke customisation and vendor lock in

__How?__
-  Choose Software as a Service (SaaS), before Platform as a Service (PaaS), before Infrastructure as a Service (IaaS)
-  Check hosting arrangements and data sensitivity when selecting cloud solutions
-  Design exit strategy before entering cloud agreements
-  Design solutions to take advantage of cloud features, such as elastic scaling, automated spin-down

__Relates to__

[TCoP5](https://www.gov.uk/government/publications/technology-code-of-practice/technology-code-of-practice#use-cloud-first): Use cloud first

## 9. Design for interoperability

__Why?__

Interoperability enables sharing of capabilities and data between systems

__How?__
-  Service Oriented and microservice architectures maximise interoperability and re-use
-  Interfaces should be discoverable and self-describing  or documented
-  Interoperability can affect the demands on solutions, therefore designs may need to be scalable to cope with other usage

__Relates to__

- [TCoP9](https://www.gov.uk/government/publications/technology-code-of-practice/technology-code-of-practice#integrate-and-adapt-technology): Integrate and adapt technology

## 10. Use open standards

__Why?__

- Avoidance of vendor lock-in
- Lays the foundation for delivering interoperability
- Open standards facilitate interoperability and data exchange among different products or services.

__How?__

Where open standards  do not exist, create one or find the best fit with least lock in

__Relates to__

- [TCoP4](https://www.gov.uk/government/publications/technology-code-of-practice/technology-code-of-practice#make-use-of-open-standards): Make use of open standards
- [SS13](https://www.gov.uk/service-manual/service-standard/point-13-use-common-standards-components-patterns): Use and contribute to open standards, common components and patterns

## 11. Design for portability

__Why?__

- Avoidance of vendor lock-in
- Moving to a new platform is simpler and requires less engineering

__How?__
- Design must be platform agnostic
- Minimise use platform specific features
- Will require an exit strategy

## 12. Design loosely coupled solutions

__Why?__

- Loosely coupled components can be replaced with alternative implementations that provide the same services.
- Components in a loosely coupled system are less constrained to the same platform, language, operating system, or build environment.

__How?__
- Projects must ensure any additional coordination protocols needed are in place
- Projects must ensure consistent data synchronisation with DfE Data guidance

__Relates to__

- [TCoP9](https://www.gov.uk/government/publications/technology-code-of-practice/technology-code-of-practice#integrate-and-adapt-technology): Integrate and adapt technology

## 13. Minimise technical debt

__Why?__

Replacing or superseding a component or service without removing existing components or services increases technical debt

__How?__
- Any project delivering a technology component or service designed to supersede or replace an existing component or service must remove the existing service as part of that project
- Project budgets need to include cost of decommissioning existing solutions or include total cost  of both systems in the business case.

__Relates to__

- [SS2](https://www.gov.uk/service-manual/service-standard/point-2-solve-a-whole-problem): Solve the whole problem for a users
