---
category: profession
expires: 2023-02-15
---

# Get help with architecture
> This is a prototype of a process flow to help everyone understand the steps involved in securing architecture support for your project.
> It will be used to test the steps with the actors involved, to then iterate and refine the process.
> Any comments to the [architecture profession mailbox](architecture.profession@education.gov.uk) please.

```mermaid
sequenceDiagram
    participant Requestor
    participant DDaT Business Partner
    participant Portfolio
    participant Roadmap
    participant Emergency Triage
    participant Profession

    Requestor -> DDaT Business Partner: Define the need and raise
    note over DDaT Business Partner: Is this definitely an \narchitecture need?
    DDaT Business Partner --> Profession: Seek advice
    DDaT Business Partner --> Requestor: Help to define the need
    note over DDaT Business Partner: Does this fit within \nan existing portfolio?
    DDaT Business Partner -> Portfolio: **Yes: small request**
    note over Portfolio: Identify architecture support
    Portfolio -> Requestor: Confirm support, agree statement of work
    DDaT Business Partner->Roadmap: **Yes: large request, raise canvas**
    note over Roadmap: Prioritised?
    Roadmap -> Portfolio: Yes
    note over Portfolio: Identify architecture support
    Portfolio --> Emergency Triage: If capacity issues, seek advice
    Portfolio -> Requestor: Confirm support, agree statement of work
    Roadmap -> DDaT Business Partner: No: confirm line to take (no, but...)
    DDaT Business Partner -> Requestor: Unable to meet demand

    DDaT Business Partner -> Emergency Triage: **No: raise for emergency triage**
    note over Emergency Triage: Establish portfolio\nand agree prioritisation
    Emergency Triage -> Portfolio: Confirm position
    note over Portfolio: Is support available?
    Portfolio --> Emergency Triage: Seek advice
    Portfolio --> Profession: Exceptionally, consult profession
    Portfolio -> Requestor: Yes: Confirm support, agree statement of work
    Portfolio -> DDaT Business Partner: No: Confirm line to take
    DDaT Business Partner -> Requestor: Unable to meet demand
```
