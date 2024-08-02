---
layout: default
title: "Blog"
---
<div>
  <div style="margin-top: 2em;"> # Added margin for spacing
    {% if site.show_excerpts %}
      {% include home.html %}
    {% else %}
      {% include archive.html title="Posts" %}
    {% endif %}
  </div>
</div>
