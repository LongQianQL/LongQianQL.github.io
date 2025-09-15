---
layout: archive
title: "Publications/Preprints"
permalink: /publications/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

<h2>Logic for Differential Equations:</h2>
{%assign dL = site.publications | where: 'category', 'dL'%}
{% for pub in dL reversed %}
{% if pub.authors %}
__{{pub.title}}__\
{{pub.authors}}.\
{{pub.venue}}. ({{pub.date | date: "%Y" }}) {% if pub.link %} <a href="{{ pub.link }}"><i class="fas fa-fw fa-link zoom" aria-hidden="true"></i></a> {% endif %} {% if pub.fileurl %} <a href="{{ pub.fileurl }}"><i class="fas fa-fw fa-file-pdf zoom" aria-hidden="true"></i></a> {% endif %}
{% endif %}
{% endfor %}

<h2>Computability:</h2>
{%assign comp = site.publications | where: 'category', 'computability'%}
{% for pub in comp reversed %}
{% if pub.authors %}
__{{pub.title}}__\
{{pub.authors}}.\
{{pub.venue}}. ({{pub.date | date: "%Y" }}) {% if pub.link %} <a href="{{ pub.link }}"><i class="fas fa-fw fa-link zoom" aria-hidden="true"></i></a> {% endif %} {% if pub.fileurl %} <a href="{{ pub.fileurl }}"><i class="fas fa-fw fa-file-pdf zoom" aria-hidden="true"></i></a> {% endif %}
{% endif %}
{% endfor %}

<h2>Computer-Assisted Mathematics:</h2>
{%assign auto = site.publications | where: 'category', 'auto'%}
{% for pub in auto reversed %}
{% if pub.authors %}
__{{pub.title}}__\
{{pub.authors}}.\
{{pub.venue}}. ({{pub.date | date: "%Y" }}) {% if pub.link %} <a href="{{ pub.link }}"><i class="fas fa-fw fa-link zoom" aria-hidden="true"></i></a> {% endif %} {% if pub.fileurl %} <a href="{{ pub.fileurl }}"><i class="fas fa-fw fa-file-pdf zoom" aria-hidden="true"></i></a> {% endif %}
{% endif %}
{% endfor %}

<h2>Miscellaneous:</h2>
{%assign misc = site.publications | where: 'category', 'misc'%}
{% for pub in misc reversed %}
{% if pub.authors %}
__{{pub.title}}__\
{{pub.authors}}.\
{{pub.venue}}. ({{pub.date | date: "%Y" }}) {% if pub.link %} <a href="{{ pub.link }}"><i class="fas fa-fw fa-link zoom" aria-hidden="true"></i></a> {% endif %} {% if pub.fileurl %} <a href="{{ pub.fileurl }}"><i class="fas fa-fw fa-file-pdf zoom" aria-hidden="true"></i></a> {% endif %}
{% endif %}
{% endfor %}

