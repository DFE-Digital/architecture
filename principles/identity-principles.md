---
category: Architecture Principles
expires: 2023-12-01
---

# Identity Principles

Identity within these guidelines refers to how our services utilise user identities to authenticate and authorise to services, and how we design and build services to ensure consistency and re-use.

Consistent use of identity platforms provides a foundation to develop joined-up end-to-end user journeys across our services, and the delivery of tailored solutions and access privileges which are linked to the user's role and aligned to their needs.

Guidance is also provided for the secure administration and management of our platforms and services, ensuring that access granted to systems is conscious and  appropriate, is granted only for the time required for the specific activity and is logged and audited.

## Identity Segment Definitions

Consumers for the Department's services are aligned to three main identity segments. This alignment enables standardisation across services and improves the experience for our users by enabling consistent end-to-end user journeys.

* **B2C** - Identity segment for services provided for citizen users who are interacting under their personal context

* **B2B** - Identity segment for services provided for sector users who are interacting under the context of their institution school/college etc

* **B2E** - Identity segment for services provided for Civil Servants, contractors and managed service providers working on behalf of Government departments

## Use of the guidelines

The following guidelines are provided to guide projects and teams when creating or procuring solutions for use by the Department's users or consumers. The guidelines will be used to create a framework for projects to operate within and to demonstrate alignment with best practice.

**Aligment and exceptions** to the principles will be reviewed as part of assurance processes with the security and architecture professions to streamline governance, Exceptions will be approved or declined as relevant, with all decisions tracked with rationale for future reference.

**Updates or modifications** to the principles can be requested initially via the Identity Community of Interest, and in the future with standard updates and iterations via GitHub.

## 1. Align to a strategic authentication service

*All systems must integrate with a strategic authentication
service.*

### Why?

By aligning with a strategic authentication service we simplify the end-user experience by being able to re-use the same identity to authenticate to multiple services. Security is improved by centralising access records and providing a single identity point to manage and maintain.

**Formal patterns are being developed at present with further information for adoption of standard services. In lieu of the formal patterns, high-level alignment to shared sevices is shown below:**

* B2C - Use the GDS One Login For Government Service
* B2B - Use DfE Sign-In
* B2E - Use AzureAD and leverage **AzureAD B2B** to invite guests

### How?

* Review strategic patterns for authentication services

* Ensure that new COTS capabilities support integration into strategic
    authentication services

* Develop using approved platforms and languages which support
    integration into strategic authentication services

* Update existing capabilities to integrate into strategic authentication services

* Retire capabilities which cannot support integration into strategic
    authentication services

## 2. Support open standards

*Open Standards ease integration burden on services, enable us to move at pace for functional and security related changes whilst ensuring knowledge to integrate with and maintain ID Systems is easy to come by*

### Why?

* We maintain alignment with the architecture principles <https://github.com/DFE-Digital/architecture/blob/master/principles/enterprise-architecture-principles.md#10-use-open-standards>

* Open Standards ease integration burden on services

* They enable us to move at pace for functional and security related changes

* The use of open standards ensures that knowledge to integrate with and maintain ID Systems is easy to come by

### How?

* When building a new service, build it on the foundations of Open ID Standards such as OAuth, OIDC or SAML

* When buying a service, make sure if conforms to the Open Standards existing ID management software within the Department / Gov adheres too.

## 3. Use data responsibly

*Data used within identity platforms to identify users must be used appropriately and in line with our standard principles*

### Why?

* Responsible use of our user's data helps to build trust with the Department and our services

* We have regulatory and legislatory responsibilities to meet and demonstrate

* We should be transparent on how data is used

* Users should be able to update and remove their data as they see fit, controlling where it’s shared and how it is captured between systems

### How?

* Follow our existing data principles and guidance.

<https://github.com/DFE-Digital/architecture/blob/master/principles/enterprise-data-architecture-principles.md#6-data-use-is-ethical>

## 3. Use data masters to enable persistence and portability and reliability

*Services should agree on attributes that can be used to mirror/merge/reference user data across many systems, enabling gaps to be easily bridged as users move between disparate systems*

### Why?

Utilising master data sources enables consistent and joined-up user experiences as we have a better understanding of our users and their roles, and are able to provide appropriate services to them and manage their access appropriately.

### How?

* Follow our existing principles for data mastering and re-use
<https://github.com/DFE-Digital/architecture/blob/master/principles/enterprise-data-architecture-principles.md#1-data-is-an-asset>

* Clearly document the attributes your service holds that future services may use to join up identities

* Work with other service and data teams to ensure the unique attributes stored within your system align with what other services are using to increase the likelihood of overlapping identity attributes

## 4. Consider the user experience

*Considering user needs is core to everything we do, and must therefore also be considered for how we manage a user's identity access journey*

### Why?

The User Experience should be considered when utilising Identity Managent solutions
How will it affect the user journey
Is it a seamless experience or does it add burden to the user?

### How?

* Follow existing guidance from the Service Manual - <https://www.gov.uk/service-manual/service-standard/point-1-understand-user-needs>

* Work with User Researchers and Product Owners across the department and Government to understand what knowledge exists today around ID and share your users challenges wider to gather critique

## 5. Consider end-user autonomy and self-service

*Systems should implement self-service capabilities to empower end-users and reduce support costs*

### Why?

Legacy systems and operational processes relied upon paper-based
processes managed by service desks to manage access to systems and make
changes. This causes delays for end-users and drives up support costs
for operatives who need to manage the end-to-end process to grant and
manage access to systems and data.

Modern Identity Governance and ITSM platforms can automate this process
either with system and data owners as gatekeepers who approve digital
requests, or automatically granting access to systems and data based on
an end-user's persona, job role or organisation.

The use of digital processes and self-service for end-users increases
end-user experience, reduces support costs and also improves security
and auditing for a system as digital audit logs can be reviewed and
governed more easily than paper-based equivalents.

### How?

* Ensure systems support principles to align to standard
    authentication and identity governance solutions and support
    policy-based access controls

* Ensure that data and system owners are identified and maintained to
    support any approvals for self-service requests

* Enable integration into ITSM platforms where relevant to allow for
    access to be automatically granted via service tickets or as part of
    standard JML processes

## 6. Consider and support access from multiple platforms

*Systems must support strategic authentication from all platforms
used to access.*

### Why?

Modern systems, both COTS and in-house developed, require access from a
range of device types (laptop, phone, tablet etc) and use-cases
(internal, supplier, citizen etc) which will utilise different methods
of access.

The system must support a consistent identity and authentication method
to be used regardless of how it is accessed and by whom.

### How?

* Evaluate the access requirements from persona and devices as part of the Discovery phase

* Ensure that access methods and use-cases are included in selection
    criteria for COTS products

* Develop systems which support the required use-cases and access
    methods

* Do not align to internally-focussed authentication services (Active Directory) if the system is
    intended to be used outside of the Department by 3rd party users

## 7. Support an approved authentication method

*Systems must utilise modern and secure authentication protocols
which are replay-resistant.*

### Why?

Modern authenticate protocols provide greater levels of security against
common attacks and malicious activity and are supported by the strategic
authentication providers.

Legacy protocols are prone to common attacks which can lead to system
compromise and data loss. Ongoing use of legacy protocols will create a
dependency with legacy authentication providers, or weakening of
security due to retaining support for legacy protocols.

### How?

* Review strategic patterns for authentication methods

* Ensure that authentication methods are included in selection
    criteria for COTS products

* Develop using approved platforms and languages which support
    integration into strategic authentication services

* Update existing capabilities to integrate into strategic authentication services

* Retire capabilities which cannot support integration into strategic
    authentication services

## 8. Provide end-to-end encryption

*Systems must protect the end-to-end communications between the
system and consumer to prevent common attacks and protect data*

### Why?

Many malicious activities involve monitoring network activity with
commonly available tools to gather credentials and system data. Modern
protocols do not expose data as they provide a level of encryption
within the authentication token, but older authentication protocols and legacy methods (username/password) could expose data which could be exploited to gain access by
impersonating a user.

End-to-end encryption is common when accessing external systems but
must also be implemented as standard for internal systems to protect
against any insider threats within the Department.

### How?

* Enable transport-level encryption for all communications between
    consumer and system and system to system

* Ensure the protocol used is secure and supported

* Ensure that ongoing support for the system includes the ongoing
    management of certificates and processes to renew and upgrade
    as necessary

## 9. Provide a mature and appropriate access model

*Systems must utilise a suitable access model so that it can be
secured and managed appropriately.*

### Why?

An access model is utilised to ensure that administrators and consumers
of a system are granted the appropriate level of access aligned to their
requirements. The levels of access and the roles provided should be
appropriate to the relevant system and the data or control it grants
access to.

A relatively simple system may only require roles for user,
administrator and approver, whereas a system managing access to
confidential data across multiple education establishments would require
a rich access model to manage both role access and to segregate data
access accordingly.

### How?

*  Review requirements for the access model as part of the Discovery phase, taking into account the data being accessed and by whom

* Review and agree the appropriate access model **in advance** with the relevant compliance teams as required to ensure that the model is developed in-line with the wider solution and not as a post-development activity

* Utilise existing measurements such as Levels of Assurance to review the appropriateness of the access model within a system

* Ensure that the security model is reviewed as part of the selection criteria for COTS products

* Ensure that COTS and in-house developed systems provide a flexible and extensible access model which can be updated and amended as required

## 10. Support role segregation and separation of duties

*Systems must utilise a role model which ensures that roles are
managed and segregated appropriately*

### Why?

Many systems include workflows to support processes for approval, code
promotion and changes to data held within. Separation of duties (SoD)
refers to the checks and balances within a process to ensure that the
relevant governance and approvals are carried out.

Separating the steps of a workflow or approval process ensures that a
task such as code promotion, approval of additional privilege or
granting access to an application or data set is suitably scrutinised.

Individuals should not be able to approve end-to-end lifecycle activity
or promote their own access rights unless there has been a conscious
decision to do so. Self-promotion or self-approval may be suitable for
specific low-privilege or low-impact activities, but this must be
reviewed with assurance teams to ensure that it is deemed as acceptable.

### How?

* Ensure alignment with principle 5 to provide a mature access model which will be sufficiently granular to support SoD

* Review workflows and approvals required within the system and capture roles and SoD details within system designs

* Ensure any self-promotion or self-approval processes and workflows are reviewed and approved by assurance teams

## 11. Adhere to least-privilege model

*Roles and privileges assigned to systems must be appropriate for
the user's requirements.*

### Why?

Providing permissions and access which are aligned to the end-users
requirements ensure that access to data is protected appropriately and
avoids the ability for malicious activity or accidental misuse.

An administrator who is provided with full access to a system for
simplicity or due to a poorly-designed access model could inadvertently
or otherwise cause damage to the system or access data inappropriately.

Managing access to the least-privilege model also ensures that impacts
from malicious activity from a stolen or impersonated account are
restricted.

### How?

* Do not use generic built-in roles for systems (domain admin, owner,
    administrator etc)

* Ensure that the security model is reviewed as part of the selection
    criteria for COTS products and supports least-privilege

* Ensure that internally-developed systems provide a granular permissions model which supports least privilege

* Ensure that COTS and in-house developed systems provide an
    extensible access model which can be updated and amended as required

* Manage the use of high-privilege roles appropriately, with
    time-bound access or with separate 'break-glass' accounts

## 12. Enable just-in-time access for administrative permissions

*High-privilege and high-access roles must be assigned on a time-bound
basis and used appropriately and only when required*

#### Why?

Accounts which carry large amounts of privileged access are targets for
malicious activity and in appropriate use. A malicious user who was able
to gain access to an account which included numerous administrative
roles would be able to cause significant damage within the Department.

Assigning roles using a just-in-time model ensures that administrators
and privileged users are provided with the access required but only when
required. The security for this can be further enhanced by using
multi-factor authentication to ensure that administrators verify the
access request appropriately.

The use of just-in-time access also instils more mature working
practices, as administrators need to plan changes appropriately and are
consciously using administrative permissions appropriately. It also
avoids the potential of accidental misuse by ensuring that the
permissions are applied explicitly rather than implicitly.

### How?

* Ensure that COTS products are selected which can either integrate
    into existing security capabilities which can provide JiT access or
    which can support JiT access natively

* Ensure that internally-developed products integrate into existing
    security capabilities which can provide JiT access

* Provide a support model which includes full alignment to the JiT
    access model with defined approvers for access requests if necessary

## 13. Secure system and machine accounts

*System accounts are powerful and must be managed and secured
appropriately to avoid misuse or malicious exploit.*

### Why?

System (aka service) accounts are used for system-to-system access or to
run unattended activities within a system, and often require
high-privileged access to do so. The system accounts often have a
password which is set once and rarely updated, which can lead to either
future exploit if this password is identified or system outage if
maintenance is required by the password is no longer known.

System accounts are often assigned unnecessarily high-privileges by the
system owners or developers for expediency rather than applying the
correct least-privilege level of access. Due to this they are often
targeted by malicious users as they can be used to gain significant
levels of access without detection.

### How?

* Ensure that system accounts are identified within system designs
    with details of the permissions assigned and usage so they can be
    monitored for anomalous activity

* Ensure that permissions assigned to system and machine accounts
    align to least privilege and are not given generic administrative
    access

* Use Managed Service Accounts on Windows platforms if compatible

* Use complex passwords which are stored securely and not shared

* Do not allow interactive login to ensure that the accounts can only
    be used for its intended purpose

* Ensure that operational processes are established for maintaining
    the accounts and resetting credentials on a 6-12 month basis

## 14. Utilise policy-based access controls

*Systems should consider policy-based and attribute-based access
controls to provide modern and flexible access methods*

### Why?

Traditional role-based access control (RBAC) methods of managing access
to systems provide granular access models and methods to ensure that
access is commensurate for the end-user. However, they do require
additional ongoing management to maintain the correct group membership
and ensure that permissions are not being collected and retained
unnecessarily.

A future move to policy-based access control systems provides greater
flexibility and adaptive controls which will change automatically as the
end-user's attributes change (job role, provider etc).

The use of policy-based access controls requires a reliable set of
master data records and therefore may not be possible for all attributes
at present, but in-house development and COTS systems should consider
this requirement so they can be adapted in the future.

### How?

* Ensure that COTS and in-house developed apps can support modern
    policy-based and attributed-based authentication models

* Architect systems for delegated controls where the Identity platform
    provides authentication and coarse-grained access and the
    applications retains responsibility for fine-grained access via user
    attributes

## 15. Design the access model for growth

*Systems must provide the ability to extend the access model for
additional access and use-cases without re-architecting*

### Why?

Systems may start with a small user community with simple access
requirements, but this will inevitably grow to accommodate more users
with potentially more complex access requirements to segregate roles and
data held within.

The business case for the relevant system should include details of the
end-state which will include the potential scale and use, and this
should be reflected not just to the application and system architecture
but also the access model to ensure that this remains fit for purpose in
the future.

### How?

* Ensure the full scope of the system is understood and captured
    within the system design and as part of the selection criteria

* Ensure that the access model is granular where required to support
    future expansion of the service to accommodate additional users,
    use-cases and data separation

## 16. Support relevant secure separation requirements

*Data held within systems must be segregated to enable access
controls and support potential future divestment or separation
requirements*

### Why?

Data held within systems will contain end-user identifiable and
sensitive information which must be segregated and protected accordingly
so that access controls can be enforced.

The architecture of the system must also support requirements for future
potential separation or divestment within the Department. The separation and
segregation within the system should ensure that data relating to
specific organisations or providers can be identified and extracted as
required.

This segregation will also support the principle to ensure the access
model for a system can enforce data separation accordingly.

### How?

* Ensure that data architecture within the system supports the
    separation between organisations, consumers etc

* Ensure that data within the application can support extraction and
    removal of specific data types without requiring re-architecture of
    the solution

## 17. Ensure access model can support multiple domains and organisations

*Systems must provide the ability to enable and control access
across diverse user types and organisations*

### Why?

Consumers of the Department's systems are located across multiple organisations
within the Department and externally. Systems providing services must therefore
support the ability to recognise the different types of users and be
able to manage access appropriately by segregating access logically
within the applications and/or the data stores used by the system.

### How?

* Ensure the architecture of the selected or developed system supports
    logical separation at sufficiently robust level for the data held
    within

* Ensure the access model within the system can leverage attributes
    held within the Identity Management platform to make access
    decisions based upon at least organisation and user role

## 18. Consider requirements for Multi-Factor Authentication

*Systems should utilise additional authentication factors as
standard to protect against malicious activity*

### Why?
MFA is often considered an additional control required when accessing systems as an administrator or when accessing high-value data which needs to be protected. However, it should be seen as a more general measure which is used to protect access to systems provided by the Department. The use of MFA has multiple benefits, not just for accessing administrative roles or high-value data.

* MFA serves as a conscious reminder that a user is accessing a system which requires additional verification to access. This may make the user more aware of their responsibilities and consider how and where they are accessing a system

* Common malicious attacks against systems utilise password brute-force attacks to attempt to guess a user's credentials and gain access. The use of MFA will stop this attack as system access will require both a username/password and an MFA challenge

* Users and suppliers will often share credentials for convenience, allowing multiple people to access the same system using the same username/password. The use of MFA restricts this poor practice as it provides the 'something you have' authentication challenge, which may be a secure token, an SMS code or a prompt on a user's mobile phone.

### How?

* Discuss and review requirements for MFA as part of the system's discovery phases, and review with an Information Security colleague if necessary to confirm whether it is a hard requirement
* Consider MFA requirements when a system undergoes a significant change to scope, such as the addition of new functionality and/or access to additional data
* Consider the platforms used to access the system (**Principle 2**) and review if MFA would be supported on all platforms. If not possible across all platforms, review a two-tier approach for access, with platforms unable to support MFA only given access to a sub-set of functionality and/or data

## 19. Integration into central reporting/SIEM for auditing

*Systems must integrate into the Department's SIEM platform to provide security oversight and assurance*

### Why?

Whilst individual system owners or teams have a responsibility for the security of their systems, the Cyber and Information Security division have a Department-wide responsibility to monitor for and protect against malicious activity and cyber threats. Integrating systems into the Department's SIEM platform provides the broad visibility of the health of all systems and enables the ability to discover and monitor any emerging threats and vulnerabilities across the estate.

### How?

* Alignment to **Principle 1** enables integration and logging for the authentication into a system, as this is provided as part of the service
* Follow standard DSAM processes to ensure the InfoSec team are aware of any sensitive data or access within the system
