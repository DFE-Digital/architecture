---
category: Standards
expires: 2022-06-12
---

# Technical standards in DfE

Like all UK Government departments, architects in DfE are guided by the [UK Government Service Standard](https://www.gov.uk/service-manual/service-standard), the [Technology Code of Practice](https://www.gov.uk/government/publications/technology-code-of-practice/technology-code-of-practice) and the [Government Functional Standards](https://www.gov.uk/government/collections/functional-standards).

Architects in DfE should also be familiar with our [Enterprise Architecture principles](../principles/enterprise-architecture-principles.md), [Technical Architecture principles](https://technical-guidance.education.gov.uk/principles/architecture/#technical-architecture-principles) and [Enterprise Data Architecture principles](../principles/enterprise-data-architecture-principles.md). 

Architects involved in developing software should also be familiar with our [coding principles](https://technical-guidance.education.gov.uk/principles/coding-principles/) and [front-end development principles](https://technical-guidance.education.gov.uk/principles/frontend-development-principles/).

## Standards in development

Some technical standards [have already been published](#published-standards), but require work to make them fit-for-purpose across DfE. Most technical standards do not yet exist or are in development.

The architecture team are co-ordinating the creation of technical standards in DfE. The following list shows proposed technical standards - derived from the [Technology Reference Model](https://educationgovuk.sharepoint.com/:f:/r/sites/gp/WorkplaceDocuments/Reference%20architecture/Technology%20Reference%20Model) and grouped by component - and who owns them.

We're working with these owners and teams to prioritise creation of the standards that will provide the most value to both delivery teams and DfE. The ones actively being working on are in **bold**. As standards are agreed and published, they will be updated on this page.

## Accepted products

Whilst technical standards are being developed, some accepted products in DfE have been highlighted against some of the higher priority groups. These are products that are currently in use in the department and make most sense to use / re-use. If you choose one of these products, you are *most likely* to be aligned with the standard being developed. More will be added as more data is gathered and analysed

### Management components

#### Strategic Management

| Group                        | Standard                                 | Product                    | Division                    |
|------------------------------|------------------------------------------|----------------------------|-----------------------------|
| Strategy Development         |                                          |                            |  DDaT Senior Leadership Team |
| Goals and Outcomes           |                                          |                            |                             |


#### Security Management

| Group                        | Standard                                 | Product                    | Division                   |
|------------------------------|------------------------------------------|----------------------------|----------------------------|
| Perimeter and Network Security|                                         |                            | Networks                   |
| Device Security              |                                          |                            | End User Compute Services  |
| Virus and Malware Prevention and Management|                            |                            | Cyber Security             |
| Data/Communication Security and Confidentiality|                        |                            |                            |
| Platform and System Security |                                          |                            |                            |
| Vulnerability and Threat Management |                                   |                            |                            |
| **Identity and Access Management** | Business to Citizen/Consumer (B2C) | *GOV.UK One Login          |                            |
|                              | Business to Business (B2B)               | *DfE Sign in               |                            |
|                              | Business to Enterprise/Employee (B2E)    | *MS Azure Active Directory |                            |
| Security Incident Management |                                          |                            |                            |
| Monitoring, Traceability, Auditing and Forensics|                       |                            |                            |

#### System Management

| Group                        | Standard                                 | Product                    | Division                   |
|------------------------------|------------------------------------------|----------------------------|----------------------------|
| Service Desk and CMDB Tools  |                                          |                            | End User Compute Services  |
| Deployment, Audit and Inventory |                                       |                            | Service Operations         |
| **Monitoring and Event Management** |                                   |                            |                            |
| Performance and Capacity Management |                                   |                            |                            |
| Mobile Device Management     |                                          |                            | End User Compute Services  |
| Device Management and Configuration Tools |                             |                            |                            |
| Remote Control Management Tools |                                       |                            |                            |

#### Delivery Management

| Group                        | Standard                                 | Product                    | Division                   |
|------------------------------|------------------------------------------|----------------------------|----------------------------|
| Portfolio and Project Management |                                      |                            | Delivery Management        |
| Architecture Management      |                                          |                            | Architecture               |
| Roadmap Development and Management |                                    |                            | Strategy & Engagement      |
| Performance Metrics          |                                          |                            | Delivery Management        |
| Service Catalogue            |                                          |                            | Service Operations         |
| Resource Capacity Management |                                          |                            | Capability                 |
| Prioritisation               |                                          |                            | Strategy & Engagement      |

#### Application Development

| Group                        | Standard                                 | Product                    | Division                   |
|------------------------------|------------------------------------------|----------------------------|----------------------------|
| **Development Tools**        |                                          | *MS Visual Studio          | Infrastructure & Platforms |
|                              |                                          | *VS Code                   |                            |
|                              |                                          | *Azure DevOps              |                            |
| **Data Access Tools**        |                                          |                            |                            |
| **Scripting Tools**          |                                          |                            |                            |
| Modelling and Design Tools   |                                          |                            | Architecture               |
| Requirements Management Tools |                                         |                            | Business Analysis Community |
| **Programming Languages**    |                                          | *C# .NET                   | Infrastructure & Platforms |
| Testing Tools                |                                          |                            |                            |
| Source Code Management Tools |                                          | *Github                    |                            |
| Lifecycle and Configuration Management Tools |                          |                            |                            |



### Devices and peripherals

#### End User Devices

| Group                        | Standard                                 | Product                    | Division                   |
| -----------------------------| -----------------------------------------| ---------------------------|----------------------------|
| Desktop Devices              |                                          |                            | End User Compute Services  |
| Laptop Devices               |                                          |                            |                            |
| BYOD                         |                                          |                            |                            |
| Mobile Devices               |                                          |                            |                            |
| Tablet Devices               |                                          |                            |                            |
| End User Device OS           |                                          |                            |                            |

#### Peripherals

| Group                        | Standard                                 | Product                    | Division                   |
|------------------------------|------------------------------------------|----------------------------|----------------------------|
| Printers                     |                                          |                            |End User Compute Srvices    |
| Scanners                     |                                          |                            |                            |
| Other Devices                |                                          |                            |                            |

#### IOT Devices
| Group                        | Standard                                 | Product                    | Division                   |
|------------------------------|------------------------------------------|----------------------------|----------------------------|
| Edge Devices                 |                                          |                            |End User Compute Services   |


### Application components

#### Business Applications

| Group                        | Standard                                 | Product                    |Division                    |
|------------------------------|------------------------------------------|----------------------------|----------------------------|
| Finance and Accounting Applications |                                   |                            |                            |
| Human Resource Management Applications |                                |                            | Human resources            |
| Sales, Purchasing and Commercial Applications |                         | *Jaeggar                   | Customer Experience        |
| Marketing Applications       |                                          | *GOV.UK Notify             |                            |
|                              |                                          | *MailChimp                 |                            |
|                              |                                          | *SendGrid                  |                            |
|                              |                                          | *SurveyMonkey              |                            |
| **Customer Service Applications** |                                     | *MS Dynamics 365           | End User Compute Services  |
|                              |                                          | *Zendesk (Customer Service Desk) |                      |
| Case Management Applications |                                          |                            | Infrastructure & Platforms |
| Business Operations Management Applications |                           | *MS Power Automate         | Business Operations        |
|                              |                                          | *MS Azure Data Factory     |                            |
|                              |                                          | *MS Forms (Data Capture)   |                            |

#### Productivity Tools

| Group                        | Standard                                 | Product                    | Division                   |
|------------------------------|------------------------------------------|----------------------------|----------------------------|
| **Collaboration Applications** |                                        | *MS Teams                  | End User Compute Services  |
|                              |                                          | *Slack                     |                            |
|                              |                                          | *LucidSpark                |                            |
| **Productibity and Office Applications** |                              | *MS Office 365             |                            |
| Email and Calendar Applications |                                       |                            |                            |
| Common Desktop Tools         |                                          |                            |                            |
| Instant Messaging and Presence Applications |                           |                            |                            |
| Document Management and Workflow Applications  |                        | *MS SharePoint             | Knowledge & Information Management |
|                              |                                          | *MS Power Automate         |                            |
| Browser and Web Desktop Applications |                                  |                            | End User Compute Services  |
| Content Management Applications |                                       | *Contentful                |                            |
|                              |                                          | *GOV.UK Publisher          |                            |
| Enterprise Search Applications |                                        |                            | Knowledge & Information Management |
| **Accessibility Applicatons** |                                         |                            | Accessibility              |
| Video and Telephony Conferencing Applications |                         |                            | End User Compute Services  |
| Digital Signature Tools      |                                          |                            | Cyber Security / Service Operations |

#### Middleware

| Group                        | Standard                                 | Product                    | Division                   |
|------------------------------|------------------------------------------|----------------------------|----------------------------|
| **API Management**           |                                          |                            | Infrastructure & Platforms |
| **Container Management**     |                                          |                            |                            |
| Enterprise Service Bus       |                                          |                            |                            |
| Message/Event Stream Processing |                                       |                            |                            |
| Middleware connectors        |                                          |                            |                            |
| IOT Platforms                |                                          |                            |                            |

### Data components

#### Analytics and Reporting

| Group                        | Standard                                 | Product                    | Division                   |
|----------------------------- |------------------------------------------|----------------------------|----------------------------|
| Data Warehouse Systems       |                                          |                            | Data Architecture          |
| Dashboard Reporting          |                                          |                            |                            |
| Operational/Transactional Reporting |                                   |                            |                            |
| Analytical Reporting         |                                          |                            |                            |
| Advanced Analytics Platforms |                                          |                            |                            |
| IOT Stream Analytics         |                                          |                            |                            |

#### Data Platforms

| Group                        | Standard                                 | Product                    | Division                   |
|------------------------------|------------------------------------------|----------------------------|----------------------------|
| **Relational Database Management Systems** |                            | *MS Azure SQL              |                            |
|                              |                                          | *PostgreSQL                |                            |
| Unstructured Data Management Systems |                                  |                            |                            |
| Analytical Data Management Systems |                                    |                            |                            |
| Data Integration and Orchestration Systems |                            |                            | Data Engineering           | 
| Data Transfer and Transformation Systems |                              |                            |                            |
| Data Connectors              |                                          |                            |                            |
| Data Governance and Quality Systems |                                   |                            | Data Architecture          |
| **Master Data Management**   |                                          |                            |                            |

### Infrastructure components

#### Server Platform


| Group                        | Standard                                 | Product                    | Division                   |
|------------------------------|------------------------------------------|----------------------------|----------------------------|
| Server Hardware              |                                          |                            | Infrastructure & Platforms |
| Server OS                    |                                          |                            |                            |
| Server Virtualisation Platform |                                        |                            |                            |
| File and Print Services      |                                          |                            |                            |
| High Availability Platform Services |                                   |                            |                            |
| Application Virtualisation Platform |                                   |                            |                            |

#### Storage and Backup

| Group                        | Standard                                 | Product                    | Division                   |
|------------------------------|------------------------------------------|----------------------------|----------------------------|
| Storage System               |                                          |                            |                            |
| Data Management and Replication |                                       |                            |                            |
| Backup and Recovery          |                                          |                            |                            |
| Network Attached Storage     |                                          |                            |                            |

#### Network and Telecoms Management

| Group                        | Standard                                 | Product                    | Division                   |
|------------------------------|------------------------------------------|----------------------------|----------------------------|
| Network Event and Fault Management |                                    |                            | Networks                   |
| Network Configuration Management |                                      |                            |                            |
| Voice/Video Management Tools |                                          |                            | End User Compute Services  |
| Network Performance and Capacity Management |                           |                            | Networks                   |
| Wireless LAN Management      |                                          |                            |                            |
| Conferencing Management Tools |                                         |                            | End User Compute Services  |

#### Network and Telecoms Infrastructure

| Group                        | Standard                                 | Product                    | Division                   |
|------------------------------|------------------------------------------|----------------------------|----------------------------|
| LAN Services                 |                                          |                            | Networks                   |
| WAN Services                 |                                          |                            |                            |
| Voice Services               |                                          |                            |                            |
| Video Services               |                                          |                            |                            |
| Wireless Services            |                                          |                            |                            |
| Conferencing Services        |                                          |                            |                            |

#### Data Centre and Facilities

| Group                        | Standard                                 | Product                    | Division                   |
|------------------------------|------------------------------------------|----------------------------|----------------------------|
| Racking                      |                                          |                            | Infrastructure & Platforms |
| Facilities Management        |                                          |                            | Estates                    |
| Fire Protection              |                                          |                            |                            |
| Physical Security            |                                          |                            |                            |
| Cabling Management           |                                          |                            |                            |
| Environment Management       |                                          |                            | Infrastructure & Platforms |

## Published standards

Whilst technical standards are being developed, architects may also find the following information useful in their work:

- [API standards](https://technical-guidance.education.gov.uk/guides/api-guidance/#dfe-api-standards)
- [Software development standards](https://technical-guidance.education.gov.uk/standards/), including things like [naming things](https://technical-guidance.education.gov.uk/standards/naming-things/), [storing source code](https://technical-guidance.education.gov.uk/standards/storing-source-code/) and [licensing software](https://technical-guidance.education.gov.uk/standards/licencing-software-or-code/)
- [Data policies and standards](https://educationgovuk.sharepoint.com/sites/lvewp00085/SitePages/DfE-Data-Policies.aspx)
- [Information security assurance](https://educationgovuk.sharepoint.com/sites/how-do-i/SitePages/security-assurance.aspx)
- Guidance on [meeting accessibility requirements](https://www.gov.uk/guidance/accessibility-requirements-for-public-sector-websites-and-apps#meeting-accessibility-requirements) and the [technical standard for digital accessibility](https://www.gov.uk/guidance/public-sector-website-and-mobile-application-accessibility-monitoring#technical-standard-for-digital-accessibility)

## Standard owners

Every standard has an owner. This is typically a technical lead in a particular domain.

A standard owner's responsibilities are to:

* Ensure the standard is published and available to all
* Ensure the standard is fit-for-purpose across DfE
* Consult (or facilitate consultation) with stakeholders impacted by the standard
* Ensure the standard is iterated and updated in the architecture repository

## Application of standards

The application of standards is generally assured through co-design in teams, and peer review in architecture and technical communities. There will also be checks that standards have been met during service assessment. Occasionally, there may be spot checks to ensure consistent and appropriate application of DfE technical standards.

Architects are responsible for architecture and design decisions in their respective portfolio, service or domain. They should be confident in representing these in their respective communities and any DfE governance or assurance forums. Typically, design decisions are recorded as [Architecture Decision Records (ADRs)](../architecture-documentation/#architecture-decision-records) and stored alongside other design and technical documentation (ideally in Github).
