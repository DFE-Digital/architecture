# DfE Architecture
This site documents the architecture principles, standards and guidance that we expect teams working
within the [Department for Education (DfE)](https://www.gov.uk/government/organisations/department-for-education)
to follow when designing services.

It complements the [GDS Service Manual](https://www.gov.uk/service-manual) and its
[technology section](https://www.gov.uk/service-manual/technology),
which covers service design more broadly.

It should be used in conjunction with the
[DfE Digital Technical Guidance](https://dfe-digital.github.io/technical-guidance),
when building digital services.

## Profession

- [Our architecture profession offer](profession/our-profession-offer)

## Principles

{% assign principle_groups = site.pages
  | where: "principle", true %}

{% for principle in principle_groups %}
- [{{ principle.title }}]({{ principle.url | relative_url }})
{% endfor %}

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

- [Design assurance](assurance/assurance-and-design)

## Repositories

- [DfE SharePoint repo](https://educationgovuk.sharepoint.com/sites/gp/WorkplaceDocuments)
- [DfE Digital Confluence](https://dfedigital.atlassian.net)
- [ESFA Confluence](https://skillsfundingagency.atlassian.net)

## Capability

- [Architecture Capability Framework](capability/architecture-capability-framework.md)
