---
category: reference
expires: 2027-03-05
---

# DfE Target Architecture

> **Tl;dr**
>
> The DfE target architecture separates user experience, business
> capabilities and operational data into reusable engines.
>
> -   **front-end engines** provide shared user-facing capabilities
>     and digital interfaces
> -   **business engines** implement reusable policy and operational
>     logic
> -   **data engines** provide authoritative operational datasets
>
> These engines are connected through APIs and supported by shared
> enabling platforms such as identity, integration, messaging and
> analytics.

[![Diagram showing enabling services surrounding the architecture
engines, including authentication services, API gateway, event messaging
infrastructure, analytics platforms and hosting
platforms.](../../images/target-architecture-enabling-platforms.png)](../../images/target-architecture-enabling-platforms.png)

## Introduction

The DfE Target Architecture describes how digital, data and technology
services should be structured across the department to deliver joined-up
services, make better use of data, and reduce duplication.

It provides a conceptual blueprint for how services should evolve
over time. The architecture does not prescribe specific technologies or
system designs. Instead, it defines patterns and structures that help
teams design services in a consistent and reusable way.

The target architecture supports the goals described in DfE's digital,
data and technology strategies and aligns with our [architecture principles](../../#principles). It has full support from the Chief Digital and Technology Officer (CDTO) and DDT Committee.

The target architecture helps DfE to:

-   deliver joined-up user experiences
-   reduce duplication and technical debt
-   improve agility and responsiveness
-   enable reuse across services
-   make better use of operational data


## Architecture in the DfE blueprint

The target architecture forms part of a broader digital, data and
technology blueprint used to guide strategic change across DfE.

Blueprints help organisations plan complex change by describing:

-   the outcomes they want to achieve
-   the capabilities needed to support those outcomes
-   the systems, data and technologies required
-   the roadmap for moving from the current state to the target state

Within this blueprint, the target architecture provides a **conceptual
structure for services and data**, helping teams understand how
different parts of the digital, data and technology landscape should fit together.


## Understanding DfE user journeys

DfE delivers services to a wide range of users across the education
system. These interactions can be understood through three broad types
of user journey.

**Customer journeys**, representing **services** used by:

-   the education sector
-   citizens
-   parents, teachers and learners

These services are typically designed around policy outcomes or
regulatory processes.

**Partner journeys**, representing **system-to-system interactions** with
external organisations. These typically involve:

-   integrations with school management information systems
-   APIs used by sector systems
-   data sharing with other government departments

**Business journeys** that support **internal users and operational processes**, including:

-   DfE staff
-   policy teams
-   analysts
-   operational and delivery teams

We sometimes refer to this model as the **'fidget spinner'** view of
DfE services because it shows how different types of interaction revolve
around shared data and enabling capabilities.

![Conceptual diagram showing the "fidget spinner" model of DfE services.
Three main user journeys radiate from a central core of shared data and
enabling services: customer journeys used by citizens and the education
sector, partner journeys involving system-to-system integrations and
data sharing, and business journeys used by internal DfE
staff.](../../images/target-architecture-user-journeys.png)

The model highlights that while users and services may differ, many rely
on the same underlying data and capabilities.

## From user journeys to architecture

Although services appear very different from a user perspective, many
rely on **similar underlying capabilities**, including:

-   common operational datasets
-   shared business rules
-   similar workflows and validations

Historically, these capabilities have often been implemented separately
in different systems, which has led to duplication, inconsistent data
and higher delivery costs.

The target architecture addresses this by introducing **reusable
engines** that provide shared capabilities across services.


## What is an engine?

In the DfE target architecture, an engine is a reusable service that
provides a specific capability used by multiple services across the
department.

An engine typically:

-   implements a clearly defined capability or data domain
-   exposes functionality through APIs or integration interfaces
-   is designed to support multiple services
-   provides a stable and scalable platform capability
-   evolves independently from the user interfaces that consume it


## Core components of the target architecture

![Layered architecture diagram showing the core engines used in the DfE
target architecture. A front-end engine provides shared user-facing
services. Business engines implement reusable business rules and
workflows. Data engines provide authoritative operational datasets such
as establishments or people. The engines are connected through APIs and
supported by enabling platforms including identity, integration,
messaging and analytics.](../../images/target-architecture-engines.png)

### Front-end engines

Front-end engines provides shared capability for delivering
digital services to users.

They may include:

-   identity and authentication integration
-   consistent navigation and design patterns
-   personalised service access
-   orchestration of underlying services

### Business engines

Business engines implement reusable business capabilities such as:

-   eligibility and validation rules
-   programme or funding calculations
-   application workflows
-   regulatory checks

They expose functionality through APIs so multiple services can reuse
the same implementation of policy logic.

### Data engines

Data engines provide shared access to authoritative operational
data.

Example domains include:

-   establishments (schools and providers)
-   people (learners or staff)
-   organisations
-   programmes or funding

Data engines provide:

-   consistent access to operational data
-   APIs for querying and updating information
-   reliable and scalable access to shared datasets


### Enabling platforms

Examples include:

-   identity and authentication services
-   API gateways
-   integration platforms
-   event and messaging infrastructure
-   analytics platforms
-   hosting and infrastructure services


## How services can use the target architecture

![Service interaction diagram showing an example user journey through the
architecture. A user interacts with a service through the front-end
engine. The front-end engine invokes one or more business engines to
apply policy rules or workflows. Business engines retrieve or update
operational data using data
engines.](../../images/target-architecture-engines-example.png)

A typical interaction might follow this pattern:

1.  A user interacts with a service through a **front-end engine**
2.  The service invokes one or more **business engines** to apply policy
    rules or workflows
3.  Business engines retrieve or update information through **data
    engines**
4.  Supporting capabilities such as authentication, messaging or
    analytics are provided by **enabling platforms**


## How teams should apply the target architecture

When designing services, teams should apply the target architecture in
line with these principles:

**Look for existing engines first**

Before building new capabilities, check whether an existing engine
provides the functionality required.

**Design capabilities for reuse**

If new capabilities are needed, consider whether they should be
implemented as a reusable engine rather than a service-specific
component.

**Separate user interfaces from core logic**

User interfaces should focus on user experience, while business logic
and operational data should be implemented within business engines or
data engines.

**Avoid duplicating operational data**

Where a **data engine** exists, treat it as the authoritative source
rather than creating separate copies of the same dataset.

**Design modular services**

Services should orchestrate capabilities provided by engines rather than
tightly coupling logic within a single application.


## Evolving towards the target architecture

The target architecture will emerge gradually as services evolve. Next steps include:

-   prioritising and building the first engines
-   integrating services with shared engines
-   extracting reusable capabilities from existing systems
-   introducing data engines for common datasets
-   retiring duplicate implementations over time

For more information, contact the [architecture profession](mailto:architecture.profession@education.gov.uk)
