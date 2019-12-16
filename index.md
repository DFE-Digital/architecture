# DfE Architecture
This site documents the architecture principles, standards and guidance that we expect teams working
within the [Department for Education (DfE)](https://www.gov.uk/government/organisations/department-for-education)
to follow when designing services.

It complements the [GDS Service Manual](https://www.gov.uk/service-manual) and its
[technology section](https://www.gov.uk/service-manual/technology),
which covers service design more broadly.

It should be used in conjunction with the
[DfE Digital Technical Guidance](https://dfe-digital.github.io/technology-guidance),
when building digital services.

## Service offer

  {% assign service_offer_groups = site.pages}
    | where: "service offer", true %}

  {% for service offer in standard_offer_groups %}
  - [{{ service_offer.title}}]({{_service offer.url | relative_url_}})
  {% endfor %}

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

## Governance and design

  { assign governance_and_design_groups = site.pages
    | where "governance and design", true %}

  {% for governance in governance_and_design_groups}
  -[{{ governance_and_design.title}}]({{_governance_and_design.url | relative_url}})
  {% endfor %}

## Repositories

- [DfE SharePoint repo](https://educationgovuk.sharepoint.com/sites/gp/WorkplaceDocuments)
- [ESFA SharePoint repo](https://educationgovuk.sharepoint.com/sites/ops-cto/strategyandarchitecture)
- [DfE Digital Confluence](https://dfedigital.atlassian.net)
- [ESFA Confluence](https://skillsfundingagency.atlassian.net)

## Capability

- [Architecture Capability Framework](capability/architecture-capability-framework.md)
