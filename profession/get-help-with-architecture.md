---
category: profession
expires: 2023-02-15
---

```mermaid
sequenceDiagram

  title Get help with architecture in DfE

  participant Requestor
  participant DDaT Business Partner
  participant Portfolio
  participant Roadmap
  participant Emergency Triage
  participant Profession

  Requestor->DDaT Business Partner:Define the need and raise
  note over DDaT Business Partner: Is this definitely an \narchitecture need?
  DDaT Business Partner<-->Profession: Seek advice
  Requestor<--DDaT Business Partner:Help to define the need
  note over DDaT Business Partner: Does this fit within \nan existing portfolio?
  DDaT Business Partner->Portfolio: **Yes: small request
  note over Portfolio: Identify architecture support
  Requestor<-Portfolio: Confirm support, agree statement of work
  DDaT Business Partner->Roadmap: **Yes: large request, raise canvas
  note over Roadmap: Prioritised?
  Portfolio<-Roadmap: Yes
  note over Portfolio: Identify architecture support
  Portfolio<-->Emergency Triage: If capacity issues, seek advice
  Requestor<-Portfolio: Confirm support, agree statement of work
  DDaT Business Partner<-Roadmap: No: confirm line to take (no, but...)
  Requestor<-DDaT Business Partner: Unable to meet demand

  group Emergency Triage
    DDaT Business Partner->Emergency Triage: **No: raise for emergency triage
    note over Emergency Triage: Establish portfolio\nand agree prioritisation
    Portfolio<-Emergency Triage: Confirm position
    note over Portfolio: Is support available?
    Portfolio<-->Emergency Triage: Seek advice
    Portfolio<-->Profession: Exceptionally, consult profession
    Requestor<-Portfolio: Yes: Confirm support, agree statement of work
    DDaT Business Partner<-Portfolio: No: confirm line to take
    Requestor<-DDaT Business Partner: Unable to meet demand
  end

```
