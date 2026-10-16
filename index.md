---
layout: default
---

{% capture readme %}{% include_relative README.md %}{% endcapture %}
{{ readme | replace: "](README.it.md)", "](index.it.html)" | replace: "](README.md)", "](index.html)" }}
