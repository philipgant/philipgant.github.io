- - -
layout: default
title: Featuring
permalink: /featuring/
- - -

## Featuring

Here's something which, encountered recently, innovates and surprises.

{% assign current = site.features | sort: 'date' | reverse | first %}

{% if current %}

{{ current.content }}

- - -

[Browse the archive →]({{ '/featuring/archive/' | relative_url }})
{% else %}
*No features yet.*
{% endif %}
