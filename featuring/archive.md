---
layout: default
title: Featuring — Archive
permalink: /featuring/archive/
---

## Archive

<div class="archive-grid">
{% assign sorted_features = site.features | sort: 'date' | reverse %}
{% for feature in sorted_features %}
  <a href="{{ feature.url | relative_url }}">
    <img src="{{ feature.thumbnail | relative_url }}" alt="{{ feature.title }}" loading="lazy" decoding="async">
    <span class="thumb-date">{{ feature.date | date: "%b %Y" }}</span>
  </a>
{% endfor %}
</div>

---

[← Current feature]({{ '/featuring/' | relative_url }})
