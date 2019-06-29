# DfE Architecture
This site documents the architecture principles, standards and guidance that we expect teams working
within the [Department for Education](https://www.gov.uk/government/organisations/department-for-education)
to follow when designing services.

It complements the [Service Manual](https://www.gov.uk/service-manual) and its
[Technology section](https://www.gov.uk/service-manual/technology),
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

{% assign standards = site.pages
  | where: "standard", true
  | group_by: "category" %}

{% for standard_group in standards %}
{% if standard_group.name != "" %}
### {{ standard_group.name }}
{% else %}
### General standards
{% endif %}

{% for standard in standard_group.items %}
- [{{ standard.title }}]({{ standard.url | relative_url }})
{% endfor %}
{% endfor %}

## Patterns

{% assign guides = site.pages
  | where: "pattern", true
  | group_by: "category" %}

{% for pattern_group in patterns %}
{% if pattern_group.name != "" %}
### {{ pattern_group.name }}
{% else %}
### General patterns
{% endif %}

{% for pattern in pattern_group.items %}
- [{{ pattern.title }}]({{ pattern.url | relative_url }})
{% endfor %}
{% endfor %}

## Repositories

{% assign repository_groups = site.pages
  | where: "repository", true %}

{% for repository in repository_groups %}
- [{{ repository.title }}]({{ repository.url | relative_url }})
{% endfor %}

## Capability

{% assign capability_groups = site.pages
  | where: "capability", true %}

{% for capability in capability_groups %}
- [{{ capability.title }}]({{ capability.url | relative_url }})
{% endfor %}

## Adding new guidance

Create a new Markdown file in the [DfE Architecture guidance repo](https://github.com/DFE-Digital/architecture) that follows this pattern, add a link to it
from this page, and make a pull request:

```markdown
---
category: The broader area this fits into
expires: yyyy-mm-dd (6 months from now)
---
# What you're writing about

Introduction of a couple of paragraphs to explain why what you're
writing about is important. The [title should probably be a verb, not a
noun][good-services-are-verbs] (e.g. “Storing source code”, not “Code
repositories”).

[good-services-are-verbs]: https://designnotes.blog.gov.uk/2015/06/22/good-services-are-verbs-2/

## User needs

Why do we do this? Who is it helping?

## Principles

What broad approaches do we follow when we do this?

## Tools

What specific software (commercial or open source) do we use to help us do this thing?
```

The service manual has some useful information on
[learning about and writing user needs](https://www.gov.uk/service-manual/user-research/start-by-learning-user-needs).
