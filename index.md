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

## Repositories

- [DfE SharePoint repo](https://educationgovuk.sharepoint.com/sites/gp/WorkplaceDocuments)
- [ESFA SharePoint repo](https://educationgovuk.sharepoint.com/sites/ops-cto/strategyandarchitecture)
- [DfE Digital Confluence](https://dfedigital.atlassian.net)
- [ESFA Confluence](https://skillsfundingagency.atlassian.net)

## Capability

{% assign capability_groups = site.pages
  | where: "capability", true %}

{% for capability in capability_groups %}
- [{{ capability.title }}]({{ capability.url | relative_url }})
{% endfor %}



## Adding new guidance

Create a new Markdown (.md) file in the [DfE Architecture repo](https://github.com/luke-slowen/architecture) that follows this pattern, add a link to it
from this page, and make a pull request:

```markdown
---
category: The broader area this fits into
expires: yyyy-mm-dd (6 months from now)
---
# What you're writing about

Introduction of a couple of paragraphs to explain why what you're
writing about is important. The [title should probably be a verb, not a
noun](https://designnotes.blog.gov.uk/2015/06/22/good-services-are-verbs-2/) (e.g. “Storing source code”, not “Code
repositories”).

## User needs

Why do we do this? Who is it helping?

## Principles

What broad approaches do we follow when we do this?

## Tools

What specific software (commercial or open source) do we use to help us do this?
```

The service manual has some useful information on
[learning about and writing user needs](https://www.gov.uk/service-manual/user-research/start-by-learning-user-needs).
