---
category: Components
expires: 2020-01-01
---

# Common Components

## What are they?

Common components are software or technical systems that are created once and reused many times in different services or business contexts. They could be applications, data, integration, a network, security products, hosting or something else. They are __building blocks__, typically mapped to a business or technical capability, which can be used to deliver modular services or systems of a higher order.

__Key characteristics__

Common components can be of any size but they all share the same characteristics:
1. They are designed according to common standards, principles and patterns, with independent quality assurance to ensure the principles and patterns have been applied.
2. They are designed and developed in a modular, scalable and resilient way to support ease of reuse and reliability.
3. They are mapped to a specific business or technical capability/service. This enables easy search and prevents duplication.
4. They are treated as an asset and therefore require asset lifecycle management – support wrap, continuous improvement, enhancement or replacement.
5. They are standalone but interoperable with other common components, such that change to one does not cause a ripple effect change to others.

## Why should we use them? ##

The adoption of common components can bring significant benefits to DfE and help people build better services, more quickly. Some of these benefits are:
- __Speed to market__ – reuse can save time to build, test and deliver services. We should not have to build services from scratch every time.
- __Reduced costs__ – the more we can reuse, the more we can save through reduced technical diversity or duplication, enabling us to focus our efforts on the differentiating or innovative aspects of the service.
- __Lower risk__ – building to common standards and through lifecycle management lowers the risk of failure.

## What's available? ##

We make a distinction between components _used_ to build a service and tools
to _enable_ the building of services.

### Service components ###

Domain | Component | Owner | Status
- | - | - | -
Hosting | [Cloud Infrastructure Platform (CIP)](#cip) | Saghir Akbar | Beta
Security & networks | [DfE Sign-in](#dfe-signin) | Leanna Green | Live
| Core network | Jon Gilbert | Live
Integration | [Enterprise API Management (EAPIM)](#eapim) | Saghir Akbar | Beta
Information & data | [Enterprise Data and Analytics Platform (EDAP)](#edap) | Harj Bilan | Beta
| Data collection | Harj Bilan | Live
| Postcode lookup | Harj Bilan | Discovery
| Geospatial / maps | Harj Bilan | Discovery
Applications | [Enterprise CRM Services](#crm) | Saghir Akbar | Beta
| 360 customer view | Saghir Akbar | Alpha
| Marketing Automation platform | tbc | Discovery
| Robotic Process Automation (RPA) platform | tbc | Alpha

### Common tooling ###

Domain | Component | Owner | Status
- | - | - | -
[End User Compute](#euc) | Outlook and Teams | Leanna Green | Live
| Telephony and Skype | Leanna Green | Live
| Mobile telephony | Leanna Green | Live
Service Management | Service desk toolset | Leanna Green | Live
Digital | Productivity tools (Slack, Trello, Confluence) | Ashley Stephens | Beta
Development | Dev tools (Azure DevOps, Github) | Saghir Akbar | Live
Information & data | SharePoint | Harj Bilan | Live

## How do we use them? ##

_(Note. Content is in development for the following sections)_

<a name="cip"></a>
### 1. Cloud Infrastructure Platform

The Cloud Infrastructure Platform (CIP) is Technology Directorate’s Microsoft Azure cloud hosting offer. It’s managed centrally and provides a highly flexible model that gives service lines _control_ and _consistency_ over how their business services are hosted.

At its core, CIP is a set of principles, processes, and technologies that facilitate the development and delivery of cloud computing, cloud applications, and cloud services.

__Documentation__

Read the [platform documentation](https://docs.platform.education.gov.uk/help/intro.html), that covers security, access, operations, monitoring. Note - you may need to request access.

__Support__

CIP has a support team who handle incidents and requests. For each service using the platform, a range of support services are provided. All services receive:
1. Policy support
2. Guidance for security
3. Guidance on best practice into production
4. Working hours support

Optional support services that can be requested during onboarding are:

1. Support for Azure DevOps for new users
2. More extensive support for security / firewalls
3. Guidance for Azure engineering

Read the team's [SharePoint wiki](https://educationgovuk.sharepoint.com/sites/ciog/groupdelivery/Home.aspx) for further information and ways to contact the CIP Engineering team.

You can raise an [onboarding request](https://dfe.service-now.com/serviceportal?id=sc_cat_item&sys_id=51b0b9c5db1ff7809402e1aa4b96197d&sysparm_category=19d07bc3dbff17003b929334ca9619bd) via the service catalogue.

__Roadmap__

To efficiently and effectively implement a layer of enterprise compliance and control, the DfE must:
-	Create a holistic Cloud Operating Model, meeting the needs of both the DfE and ESFA platform management and service engineering and delivery teams.
-	Create tailored principles and processes, ensuring resources offered directly by the Cloud Hosting provider (Microsoft Azure) are consumed and configured in the desired manner.
-	Define, create, and manage, a selection of services that enable, empower, and protect, delivery teams and the services created by them.
-	Ensure that services offered to the engineering and delivery teams are fit for purpose, fit for use, isolated from one another, and can be easily discovered and consumed by engineering and delivery teams.

This results in CIP being understood as “a set of documented principles and processes, underpinning a range of decoupled ‘Platform Services’, that are orchestrated and automated ensuring consistency and quality throughout”.

With this holistic operating model, definition of platform services and appropriate process orchestration, the Cloud Hosting provider (e.g. Azure, AWS, Google Cloud Platform, etc) becomes largely irrelevant, as multiple providers can be considered for use in conjunction with one another, supporting the organisation's operating model and management tool(s).

The operating model, under active development and being matured, results in a Cloud Infrastructure Platform that is consistent, understood, repeatable, flexible, secure, encompassing and controlled.

__Further guidance__

- Read the [Cloud Infrastructure and Platform Services wiki](https://educationgovuk.sharepoint.com/sites/ciog/groupdelivery/Home.aspx) on SharePoint


<a name="eapim"></a>
### 2. Enterprise API Management

[description]

__Documentation__

__Support__

__Roadmap__

__Further guidance__


<a name="edap"></a>
### 3. Enterprise Data and Analytics Platform

[description]

__Documentation__

__Support__

__Roadmap__

__Further guidance__


<a name="dfe-signin"></a>
### 4. DfE Sign-in
DfE Sign-in is the department’s strategic Identity and Access Management (IdAM) solution. DfE Sign-in already provides IdAM for services migrated from Secure Access and a number of other services that have on-boarded during 2019. All new services should use DfE Sign-in.

DfE Sign-in is an OpenID Connect Identity provider (with support for SAMLp). It is designed to serve as a delegated authority for identity management, harnessing the global experience for all users. The net result is that Service Owners don't need to build identity solutions into their services and service users don't need to maintain many sets of credentials.

Because DfE Sign-in is a standards-based identity provider, integration is simple. Many technologies and frameworks have stable integration components and examples.

__Documentation__

Our service is available at [https://services.signin.education.gov.uk](https://services.signin.education.gov.uk/)

Please read our [getting started](#) guide.

You may also find the following code repositories for services that use DfE Sign-in useful, along with some example integrations that we have built:
- [Teachers Payment Service](https://github.com/DFE-Digital/dfe-teachers-payment-service) (Ruby on Rails)
-	[Course Directory](https://github.com/SkillsFundingAgency/dfc-coursedirectory) (.NET Core)
-	[Other integration examples](https://github.com/dfe-digital/?utf8=%E2%9C%93&q=example)

__Support__

Support for DfE Sign-in is available through our [help pages](https://help.signin.education.gov.uk/contact). These pages contain useful information for users and approvers on how to use DfE Sign-in. If a user is still having problems, they can submit a support request too.

DfE Sign-in support requests are managed via a dedicated DfE Sign-in service desk where we can monitor and track support requests. That enables us to collect information to help improve the service, highlight any potential service issues and regularly update the help pages to further support our users.

Please direct your users through this support route. If there is anything you would like to discuss or be taken through common issues or regular queries, please contact the Product Manager.

__Roadmap__

You can see [who’s already using DfE Sign-in](https://services.signin.education.gov.uk/). Any staff, provider and citizen services that currently use the Pirean Access: One product will migrate across to DfE Sign-in by July 2020.

A full roadmap of services to be onboarded can be seen below:

<img src="../images/dfesignin-roadmap.png" alt="Image of the DfE Sign-in roadmap" /><vr/>

__Further guidance__
-	Product Manager - [Ravi Jassal](https://eur.delve.office.com/?u=ec77c25a-0307-40cc-9e6b-4e1d05eda0fc&v=work)
-	Delivery Manager - [James Cheetham](https://eur.delve.office.com/?u=05f12707-cf64-4928-a6da-d5b4d96c5870&v=work)
-	Product Owner - [Jane Ludlow](https://eur.delve.office.com/?u=29a68eae-0685-4e19-af80-e51da80951ae&v=work)



<a name="crm"></a>
### 5. Enterprise CRM Services

[description]

__Documentation__

__Support__

__Roadmap__

__Further guidance__


<a name="euc"></a>
### 6. End User Compute

Providing your devices, productivity and collaboration tools, including laptops and tablets, smart phones, telephony, Office 365, Skype for Business and other software, plus facilities to print, fax and scan.

__Documentation__

- Search through and read articles on the [service portal](https://dfe.service-now.com/serviceportal)

__Support__

- Talk to the Product Owners, contact details on the [Technology Directorate service offer](https://educationgovuk.sharepoint.com/sites/ciog/SitePages/Technology-Directorate-Services.aspx) pages
- All incidents and request should be raised via the [service portal](https://dfe.service-now.com/serviceportal)

__Roadmap__

- _Unified comms_
- _Desktop / productivity_

__Further guidance__


## Further guidance on common components ##

For more information on common components or to discuss adding your component to the repository, contact the [Architecture team](mailto:architecture.governance@education.gov.uk)
