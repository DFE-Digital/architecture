---
category: Standards
expires: 2020-01-01
---

# Common definitions

## How we talk about services in DFE

Our goal is to create a common set of definitions, to help us talk about services and understand what’s meant by them in the Department for Education.

It takes time to understand what everyone means when they say ‘service’, ‘product’, ‘user need’, ‘platform’, ‘channel’, ‘architecture’, ‘policy’, ‘data’ and ‘strategy’, for example, as we all have our own definitions.

The value in a common set of definitions is not so much in what the actual words are, but the fact that we made this together as a multi-disciplinary group, and that we all agree to try it out.

This will enable us to have better discussions, spot commonalities, think about design patterns and organise large portfolios of work more easily. It also provides a language to communicate how things could work differently in future.

It is also important to understand the different roles involved in using a common set of definitions.

## Different levels of work ##

The kind of work we do might be around creating a new service, optimising parts of how an existing service works, or influencing a larger programme of work or procurement or contract, that has the ability to improve (or risk of negatively impacting) parts of a service in its scope.

Here is a high-level view of some of our common definitions, with some examples of the levels of work:

![Image of Levels of Work](../images/definitions-levels-of-work.png)

## Terms and definitions ##

The terms we use in the different levels of work may have different meanings or connotations, dependent on your or your user's perspective. We’ve tried to make these definitions as generic as possible without losing meaning, or have provided contextual examples to help give meaning.

- [Service](#service)
- [Capability](#capability)
- [Product](#product)
- [Activities and tasks](#activities)
- [Technology](#technology)
- [Data](#data)
- [Common component](#common-component)
- [Platform](#platform)
- [Register](#register)

<a name="service"></a>
### Service ###

We describe a whole service as:

_“everything the user needs to do to achieve a goal. It is the end-to-end journey that helps a user to achieve something - e.g. from thinking a career in teaching to stepping into a classroom as a newly qualified teacher, from start to finish.”_

The whole service is defined from the user’s perspective, rather than from ours.  That's why in government it is standard practice to name services by how a user would think of them or search for them online - eg ‘get a passport’, ‘become a teacher’, ‘learn to drive’ or ‘become an apprentice’.

In DfE, a user could be a student, a parent or guardian, a child, an external training provider, a civil servant - anyone that needs to do something, where they or government has a particular outcome to achieve.

A service is a collection of 'things' that users interact with that help them achieve their goals. As a result, a service entails an ongoing and consistent relationship between an organisation and its users. ‘Things’ could be digital products, call centres that offer support, business processes, communications, interaction with users - any constituent part of a whole service.

Important things to know about a service:
- They come and go
- They have a life cycle
- Digital is just one aspect of the service
- Services are continuously improved
- Services deliver policy outcomes

Services work:
- _End-to-end_ - from where a user starts to explore and understand what they have to do, to the achievement of the goal that they set out to complete
- _Front-to-back_ - meaning from where users are interacting with the service through some kind of touchpoint (face-to-face, online, phone or other), to the behind the scenes processes and systems that support them, and finally the things hidden from the user but essential to the service, such as governance and financial management aspects

![Image of aspects of a service](../images/definitions-service-aspects.png)

It can be helpful to think about these elements like a performance, with things going on in front of and behind the curtain, plus everything 'behind the scenes' to make sure the production can go ahead.

![Image of the parts of a performance, as an analogy for a service](../images/definitions-service-performance.jpg)

People often describe a map of all these things as a 'service blueprint'.

![Image of an example service blueprint](../images/definitions-service-blueprint.png)

Every service should have an owner who is responsible for improving the service, managing the day to day operations of the service and ensuring it continues to deliver value to its users and the organisation.

For more insight into services, have a look at the _#serviceowners_ and _#servicedesign_ channels on [DfE Slack](https://ukgovernmentdfe.slack.com).


<a name="capability"></a>
### Capability ###

A capability is an abstract concept, used to describe what we do (but not how). It can be thought of as all the things we need to deliver on our goals – they help us consider whether we have all the expertise, knowledge, technology, organisation and capacity to do it.

Capabilities are often categorised as:
- business capabilities, that describe what the organisation does
- people capabilities, that describe the skills,  experience and capacity people have or need to do their job
- enabling capabilities (such as technology, data) that support both business and people capabilities

DfE has a [Business Capability Model](https://educationgovuk.sharepoint.com/sites/gp/WorkplaceDocuments/Capability/DfE%20Business%20Capability%20Model.pdf), that's currently undergoing iteration.


<a name="product"></a>
### Product ###

A product enables the delivery of the service. A product is a coherent set of digital, technology, application, data, infrastructure and security components, used in the context of a service, to deliver value by addressing a specific problem experienced by users.

Generally, products are tangible items that can be acquired, sold or consumed in some way.

Example, a Customer Relationship Management product.


<a name="activities"></a>

### Activities and tasks ###

Activities and tasks are the things people do in relation to using a service, including:
- finding out how something works
- calling people for help
- applying for something
- gathering evidence
- waiting and worrying about what might happen
- being notified about a result
- calling to find out what’s happening

Activities can also describe the things that need to happen to make a service work, whether by people or by computers, for example, to achieve an outcome, such as:
- checking eligibility
- checking suitability
- making a decision
- notifying someone about a decision
- revoking permission

Activities should describe what happens, but not how it happens, by whom or with what. So, we’d use ‘notifying someone’ rather than ‘sending a letter’ and ‘making a decision’ rather than ‘casework’.

Example, a claims advisor deciding how much someone’s insurance claim is worth.


<a name="technology"></a>
### Technology ###

Technology covers the systems, tools, platforms and applications we build, maintain and buy. Technology exists to support products, activities and capabilities, enabling us to deliver faster, clearer, simpler services.

Example, a cloud hosting platform.


<a name="data"></a>
### Data ###

By data, we mean the actual information that’s either generated by or used to carry out activities and services. We try to describe what the data actually is using descriptive words, such as ‘National Insurance number’, and avoid acronyms.

Data can be thought of in two ways, operational data, which is generated by the operation of a service. An example would be completion rates on a digital service.

The second can be thought of as intelligence. Data that we consciously generate in order to make decisions. An example is customer satisfaction or census data. We ask a conscious question from our users.

Data can sometimes be provided as a service for internal or specialist end users, for example, through registers or other databases, APIs, standards and permission or usage based controls.


<a name="common-components"></a>
### Common components ###

A common component is a software or technical system that is created once and reused many times in different services or business contexts. They are building blocks, typically mapped to a business or technical capability, which can be used to deliver modular services or systems of a higher order.

Common Components can be of any size but they all share the same characteristics:
- They are designed according to common standards, principles and patterns, with independent quality assurance to ensure the principles and patterns have been applied.
- They are designed and developed in a modular, scalable and resilient way to support ease of reuse and reliability.
- They are mapped to a specific business or technical capability/service. This enables easy search and prevents duplication.
- They are treated as an asset and therefore require asset lifecycle management – support wrap, continuous improvement, enhancement or replacement.
- They are standalone but interoperable with other common components, such that change to one does not cause a ripple effect change to others.

In a mature organisation, common components allow us to build services and products more quickly. Reusing common elements from other services, such as ‘log in’, rather than recreating it multiple times, in multiple ways.
Some examples of common components in DfE are the Cloud Infrastructure Platform (CIP), DfE Sign-in for identity and access management and the Enterprise API Management platform (EAPIM).

Read more on the [common components guidance](../../common-components).


<a name="platform"></a>
### Platform ###

A platform is something you can build a product or service upon. Platforms are typically groups of technologies that, collectively, provide the basis on which applications, products, services, processes can be built.

Examples of platforms include the Cloud Infrastructure Platform (CIP) and the Enterprise API Management platform (EAPIM).


<a name="Register"></a>
### Register ###

The single place to find authoritative information on a single subject or domain. A register must have a data controller or steward who is responsible for ensuring the information contained on a register is kept up to date, accurate and accessible.

For example, the Foreign and Commonwealth Office (FCO) maintains a register of countries. It is a single, maintained list of countries. Any service can connect to this register to provide a single, consistent and authoritative list to its users.

Technology Directorate maintains a register of all Services, Products, Technology and Platforms called the Configuration Management Database (CMDB)

## Roles ##

We’re conscious that definitions of the roles involved in creating and maintaining services can sometimes be confusing - for example, does the Service Owner of a public-facing service have the same responsibilities as a Service Owner for an internal technology service?

Associated roles are defined in the [DDaT Capability Framework](https://www.gov.uk/government/collections/digital-data-and-technology-profession-capability-framework) and, depending on your feedback, may feature as part of our common definitions in the future.

## Get in touch ##

We'd love to hear your thoughts - please contact [Jack Collier](https://eur.delve.office.com/?u=b177acc8-6447-49b3-9f6c-89a1faad2ccd&v=work), [Luke Slowen](https://eur.delve.office.com/?u=fa01b414-9e39-4740-ab85-0ef228e3f7e7&v=work), [Ushma Gill](https://eur.delve.office.com/?u=976f27df-5486-4d6a-8afd-b46f95453e70&v=work) or [Paul Brown](https://eur.delve.office.com/?u=ce9e74df-d602-437b-89a4-37bd876dbaf2&v=work).
