---
layout: page
title: GSP™ Certified Organizations
---


{% for company in site.certified %}
  {%- assign cert = site.data.certification_levels | where: "id", include.level | first %}
- [{{ company.name }}]({{ company.url }}) – {{ cert.name }}.
{%- assign valid_until_ts = company.valid_until | date: "%s" -%}
{%- assign now_ts = site.time | date: "%s" -%}
{%- if valid_until_ts < now_ts -%}
 ⚠️ This certification has expired.
{%- endif -%}
{% endfor %}
