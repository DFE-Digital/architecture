---
category: Guidance
expires: 2025-12-12
---

# Business architecture best practice

In DfE, business architects may be employed in various ways, performing various tasks. Whilst there may be inconsistency in what a business architect is tasked to do, it can be useful for DfE to have accepted best practice, focused on how usual business architecture tasks might be performed.

Accepted best practice helps provide business architects with guidance when creating artefacts. It can ‘jump start’ tasks which would otherwise need scoping and support the combination and comparison of artefacts, by providing consistency if such activities are desired.

Many business architecture practices might be suggested or used in DfE. Whilst the practices offered below are considered sensible for DfE, none are mandated.

Business architects should refer to the [DfE Subject Taxonomy](https://educationgovuk.sharepoint.com/sites/lvedfe00014) and [common definitions](../common-definitions/) for terms and definitions, for descriptions of some of the ‘things’.


## Mapping

Maps are high-level visual representations of the things being mapped.

Mapping should focus on two things as a minimum - visualisation of things mapped, and the relationships and flows between them.

The purpose of mapping is to aid the understanding of, and communicate regarding, the things being mapped.

The recommended basic mapping tool in DfE is Microsoft Visio. For more complex mapping exercises, use ArchiMate compatible tools, such as [Archi](https://www.archimatetool.com/).

*What things might a business architect typically map?* Value streams, organisational structures, stakeholder relationships.


## Modelling

Models are detailed, structured representations of what is being modelled.

Modelling in the context of business architecture should focus on describing and simulating business activities, or ‘what’ an organisation does.

The purpose of modelling is to aid analysis of business activities to drive improved decision making.

The recommended basic modelling tools are Microsoft Visio or Excel. For more complex modelling exercises, use ArchiMate compatible tools such as [Archi](https://www.archimatetool.com/).

*What things might a business architect typically model?* Business capabilities, processes, information/intelligence (from data), operating models, services.


## Capability modelling

As described in [common definitions](../common-definitions/#capability), capabilities are abstract concepts used to describe *what* we do.

To deliver most value in an organisation, capability models should be comparable and therefore need to be created in a consistent manner. This ensures clarity, reliability and usability for various stakeholders and across initiatives.

In DfE, capability models should follow the guidance below:

### Categorisation

Capabilities should be categorised as [strategic, core or enabling](../common-definitions/#capability)

### Levelling

Capabilities should be levelled (decomposed), usually to 3 levels, with the following characteristics:

* Level 1 - broad scope, stable and enduring, often cut across organisational groups, can be easily decomposed
* Level 2 - operational focus, narrowing to actionable scope, relatively stable, direct ‘child’ of a level 1 capability
* Level 3 - process or task focused, specific scope, subject to regular change, direct ‘child’ of a level 2 capability

A generic example of levelling is:

|Level 1| Level 2|Level 3|
|-----------|-----------|-----------|
|Customer Relationship Management|<ul><li>Customer Segmentation and Analytics</li><li>Customer Support and Service</li><li>Customer Feedback Management</li></ul>|For Level 2 Customer Feedback Management<ul><li>Feedback Collection</li><li>Feedback Analysis</li><li>Feedback Integration</li><li>Feedback Management Tools and Platforms</li></ul>|
|Product Development|<ul><li>Ideation and Concept Development</li><li>User Research and Analysis</li><li>Product Testing and Validation</li><li>Product Lifecycle Management</li><li>Product Design and Prototyping</li></ul>|For Level 2 Product Design and Prototyping<ul><li>Conceptual Design</li><li>Prototype Development</li><li>Design Validation</li><li>Collaboration and Tools</li></ul>|
|Supply Chain Management|<ul><li>Supply Chain Risk Management</li><li>Demand Planning and Forecasting</li><li>Procurement and Supplier Management</li></ul>|For Level 2 Procurement and Supplier Management<ul><li>Bid Management</li><li>Contract Management</li></ul>|

### Scope

Avoid capabilities so broad that they include multiple unrelated areas. And/or are too abstract to provide practical value, requiring an unmanageable number of levels to decompose. For example, ‘delivering customer services’, ‘managing financial operations’ or ’developing products and services’ are all too broad. 

### Definition

Capabilities should be described to a level of detail that is easily understood and unambiguous, to ensure clarity, aid ease of use and avoid risk of duplication.
