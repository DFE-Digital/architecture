---
category: profession
expires: 2023-02-15
---

# Get help with architecture
> This is a prototype of a process flow to help everyone understand the steps involved in securing architecture support for your project.
> It will be used to test the steps with the actors involved, to then iterate and refine the process.
> Any comments to the [architecture profession mailbox](architecture.profession@education.gov.uk) please.

```mermaid
graph TD
    A(fa:fa-user Requestor) -->|Define the need and raise| B(fa:fa-handshake DDaT Business Partner)
    B --> C{Architecture need?}
    C -.-> |Seek advice| D(fa:fa-users Profession)
    D -.-> C
    C --> |No: help define the need| B
    C --> |Yes|E{Portfolio fit?}
    E --> |Yes: small request| F(fa:fa-briefcase Portfolio)
    E --> |Yes: large request, raise canvas| G(fa:fa-road Roadmap)
    E --> |No: raise for emergency triage| H(fa:fa-exclamation-triangle Emergency Triage)
    F --> |Confirm support, agree SoW| A
    G --> I{Prioritised?}
    I --> |Yes| F
    I --> |No| B
    B --> |Unable to meet demand| A
    F -.-> |Capacity issues: seek advice| H
    H -.-> F
    H --> J(Establish portfolio and prioritisation)
    J --> |Confirm position|F
```
