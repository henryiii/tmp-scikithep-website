---
layout: page
title: Documentation
permalink: /documentation
nav_order: 4
---

Documentation
=============

Please refer to the documentation provided by the individual packages.
The table below provides direct links \... Note that in
some cases the README files are the actual documentation. For certain
packages where ReadTheDocs style of documentation is available, the
READMEs still contain handy \"getting started\" sections.


| Package | README | Documentation |
|---------|--------|---------------|
{% for item in site.data.projects -%}
{%- if item[1].docs != '' -%}
{%- capture docs -%} [Read the Docs]({{item[1].docs}}) {%- endcapture -%}
{%- endif -%}
| [{{item[1].title}}](item[1].url) | [README]({{item[1].readme}}) | {{docs}} |
{% endfor %}



