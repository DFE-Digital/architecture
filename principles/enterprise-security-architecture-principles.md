---
category: Architecture Principles
expires: 2021-01-01
---

# Enterprise Data Architecture Principles

## 1. Data is an Asset
_Data is like any shared asset with value to the whole Department and beyond._

__Why?__

Data is a Departmental shared resource with a measurable value. Data is the golden thread that supports seamless, user-centric user journeys that allow users to self-serve wherever possible. Data supports decision-making at all levels from front-line delivery to policy-making and governance across the Education sector. Accurate, timely data is required to support accurate, timely decisions. Like all corporate assets, data must be carefully managed and maintained, ensuring its accuracy and reliability. Since it is the foundation of our decision making, we must have clear visibility of where it is, how good it is and the individual who owns it on the Department’s behalf, and we must be able to access it where and when we need it.

__How?__

- This principle is related to ”Data is shared,” and “Data is obtainable,” so all teams should understand the relationship between the value of data, sharing of data and accessibility to data. 
- All data should be registered in the Department’s [Data Estate Map](https://s101p01-ifax01.ad.hq.dept:8443/search/#!lineage-container) that records the legal basis on which we capture the data, how we process and use it, who owns it and the policies and privacy notices that apply to it. This will ensure we remain visibly compliant with Data Protection legislation such as GDPR.
- Data must only be used for legally permitted purposes, as defined by GDPR and captured in the [Data Estate Map](https://s101p01-ifax01.ad.hq.dept:8443/search/#!lineage-container).
- Services must work to improve the value of our shared data assets by ensuring processes are in place to maintain and improve data quality. This includes making sure data is validated by users at point of capture wherever possible, and tracking the changes to data across user journeys.
- Services must refrain from diluting the value of our data assets by creating their own versions of assets – we must agree master data sources and ensure those are always used
- We must have clear accountability for our data assets, in the form of data owners
- Our data assets must be properly managed, with responsibility for this management sitting with data stewards
- Stewards must have the authority and mechanisms to manage the data for which they are responsible
- Data stewards must ensure data quality, and should have procedures and plans to correct errors in their data and improve processes that create flawed information.
- Data quality should be measured and made visible to all users of the data.

## 2. Data is Secure
_All confidential, sensitive or personal data will be protected from unauthorised access or use_

__Why?__

The Department has a legal and moral obligation to keep personal, confidential or sensitive data secure, and we must ensure that uses and users of the data conform with this obligation. In the case of personal data in particular, we can only use it for the legal purposes for which it was collected. Pre-release access to statistical data must also be highly controlled as there are strong legal limits around what may be shared before publication, and commercially sensitive data may inhibit the Department’s ability to manage its contracts effectively if it is shared inappropriately. The Department also a large amount of children’s data, which it must safeguard.

__How?__

- We adhere to our [Data Classification Policy](https://educationgovuk.sharepoint.com/sites/lvewp00085/WorkDocs/Policies/Data%20Classification%20Policy%20v1.0.pdf?web=1), to ensure we correctly classify data stores in terms of the sensitivity of data they contain. This will include reference to cross-Government standards around data classification, but DfE specific sensitivity labelling should be used if needed.
- The Department’s [Data Estate Map](https://s101p01-ifax01.ad.hq.dept:8443/search/#!lineage-container) must be used as a central, authoritative repository for these policies. It must also record the legal basis on which we are allowed to process the data we hold and the restrictions that apply to any onward sharing or other use of the data.
- Our [Data Classification Policy](https://educationgovuk.sharepoint.com/sites/lvewp00085/WorkDocs/Policies/Data%20Classification%20Policy%20v1.0.pdf?web=1) articulates clear standards in terms of the ways data at different classification levels should be protected. We must ensure those standards are adhered to by all our services, both at design time and during service operation. Our [Handling Information Policy](https://educationgovuk.sharepoint.com/sites/how-do-i/SitePages/security-handling-information.aspx) determines who can access different classification levels.
- Security must be applied at the data level, not just the application level, and must apply equally to copies, database logs and backups.
- Security must be designed into data elements from the start of service development. Systems, data and technologies must be protected from unauthorised access and manipulation, and this protection should be tested before any release involving data assets
- A strong system of monitoring must be in place to ensure we are alerted to unauthorised access or use of the Department’s data, whether that resides in individual applications or common data stores.
- Data may be held in un-anonymised form but must be suitably anonymised before being presented to end users or removed from production security-level environments.
- This principle also relates to ‘Data is obtainable’ – we must ensure the right balance between accessibility and security

## 3. Data is Shared
_All services have data that is useful to users outside the service boundary_

__Why?__

Maintaining data in a single service then sharing in response to business/service needs has several large advantages:
- The speeding up of data collection, creation, transfer and use
- The improvement in quality and efficiency of decision-making based on timely and accurate data
- The reduction in costs of data management by eliminating duplication and synchronisation costs
- Better user journeys through re-using data the Department already holds rather than asking users to re-key
- Faster service development through re-use

__How?__

- This principle is related to ”Data is an asset,” and “Data is obtainable,” so all teams should understand the relationship between the value of data, sharing of data and accessibility to data.
- Our digital services and legacy applications must conceptually comprise a single ‘shared environment’ across which data is easily consumed between services.
- We must adhere to the common set of policies, procedures and standards for data management, discovery and access agreed by data owners and stored in the Data Estate Map.
- Services must design appropriate interfaces to their data to allow other services and users to consume their data. 
- Services should assume that the Department will need to analyse data created/collected by that service and should use the common patterns developed to enable easily passing data to the Enterprise Data & Analysis Platform.
- Data should be consistently defined throughout the Department, using definitions that are understandable and available to all users. A central data dictionary should be created and maintained as part of our Data Estate Map.
- For data to be discoverable, we must maintain a searchable central metadata repository, including data elements, data models and other metadata as part of our Data Estate Map.
- Where legally permitted, data will be available externally to further the business of government and to support wider citizen and business use of Departmental data.

## 4. Data is Obtainable
_Data is obtainable for users to carry out their activities_

__Why?__

Wide access to data means that efficient and effective decisions can be made across the whole organisation, with timely responses to data requests and service delivery. Data should be obtainable by a wide variety of users and services.

__How?__

- This principle is related to ”Data is an asset,” and “Data is shared,” so all teams should understand the relationship between the value of data, sharing of data and obtainability of data
- This principle also relates to ‘Data is secure’ – we must ensure the right balance between obtainability and security
- All users should be able to obtain data easily
- The way information is stored, accessed and presented must be adaptable for a wide range of users and their corresponding methods of access
- Obtainable data must also include good quality metadata to minimise the risk of erroneous decision-making based on a misunderstanding of the data context. Much of this will be captured in the [Data Estate Map](https://s101p01-ifax01.ad.hq.dept:8443/search/#!lineage-container), but should also include process/user journey metadata to understand how data were captured in the first place
- Good governance must be in place to ensure those with access to data understand their responsibilities under the Data Protection Act, and the limits of what they can do in the way of publishing, sharing or modifying the data. The Data Estate Map should be used to store and present this information to users.
- It must be quick and easy to determine who has access to each data asset, and to audit any human or computer access for any time period going back for a reasonable amount of time.

## 5. Data is Analysable
_Our data fundamentally underpins our ability to assess policy and delivery effectiveness_

__Why?__

Making sound policy and spending decisions across the whole Department is significantly enhanced by access to timely, accurate data from all services and across the wider educational sector. Holding this data for all systems, services, functions and processes will enable a common view on our citizen interactions, our management decisions and how our utilisation of resources best serves the tax-payer. With the Department’s increasing delivery focus, we increasingly need to have Business Intelligence and Management Information across the sector, as well as our own Financial, Commercial & HR processes.

__How?__

- Data should be gathered from all systems, services and applications and stored in the Enterprise Data & Analysis Platform (EDAP) so that analysts can easily consume and compare data from across the DfE without creating multiple analytical copies of data.
- All new systems and services will be procured or developed on the basis that they can store data within EDAP.
- Visualisation and analytics software will be provided to allow consumption of data in ways appropriate to user needs, including reports, dashboards, statistical analysis etc
- This data and its subsequent use will be covered by DfE Data Governance policies and processes, and the Government Statistical Service Code of Practice
- Data owners must define policies and processes to ensure data quality problems identified once data reaches EDAP can be reported to relevant services and data stewards to be fixed at source. See our [Data Governance Hub](https://educationgovuk.sharepoint.com/sites/lvewp00085)

## 6. Data use is Ethical
_We must process and store data in line with the ethical consensus around data use_

__Why?__

We must retain public trust in order that the Department and sector can be effective in its delivery of government services. We must therefore guard against collecting data that the public would feel exceeds ethical limits, or represents an overly intrusive reach into their private lives.

__How?__

- We must maintain a series of ethics panels to guard against overreach through a focus on efficient delivery.
- We must ensure we have consent where necessary to process data, and maintain a record of that consent. This applies to both operational and analytical uses of data.
- All the data attributes we collect should be necessary for discharging the delivery or governance responsibilities of the Department. Any more than this represents ethical over-reach.
- Care must be taken to avoid linking datasets that may be each legitimately gathered, but when combined may give an overly intrusive insight into citizens’ private lives, unless explicit consent is received to do so.
