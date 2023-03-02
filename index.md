# DfE Architecture
This site documents the architecture principles, standards and guidance that we expect teams working
within the [Department for Education (DfE)](https://www.gov.uk/government/organisations/department-for-education)
to follow when designing services.

It complements the [UK Government Service Manual](https://www.gov.uk/service-manual) and its
[technology section](https://www.gov.uk/service-manual/technology),
which covers service design more broadly.

It should be used in conjunction with the
[DfE Digital Technical Guidance](https://technical-guidance.education.gov.uk),
when building digital services.

## Profession

- [Architecture roles](profession/architecture-roles)
- [Architecture profession](profession/architecture-profession)
- [Architecture community](profession/architecture-community)
- [Architecture Capability Framework](profession/architecture-capability-framework.md)

## Principles

{% assign principle_groups = site.pages
  | where: "principle", true %}

{% for principle in principle_groups %}
- [{{ principle.title }}]({{ principle.url | relative_url }})
{% endfor %}
- [Technical Architecture Principles](https://technical-guidance.education.gov.uk/principles/architecture/#technical-architecture-principles)

## Standards

{% assign standard_groups = site.pages
  | where: "standard", true %}

{% for standard in standard_groups %}
- [{{ standard.title }}]({{ standard.url | relative_url }})
{% endfor %}

## Patterns

{% assign pattern_groups = site.pages
  | where: "pattern", true %}

{% for pattern in pattern_groups %}
- [{{ pattern.title }}]({{ pattern.url | relative_url }})
{% endfor %}

## Common Components ##

- [Common Components](common-components/)

## Design assurance

- [Design assurance](assurance/design-assurance)

## Repositories

- [DfE SharePoint repo](https://educationgovuk.sharepoint.com/sites/gp/WorkplaceDocuments)
- [DfE Digital Confluence](https://dfedigital.atlassian.net)
- [ESFA Confluence](https://skillsfundingagency.atlassian.net)




