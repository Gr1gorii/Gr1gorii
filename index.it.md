---
layout: default
---

{% capture readme %}{% include_relative README.it.md %}{% endcapture %}
{{ readme | replace: "](README.it.md)", "](index.it.html)" | replace: "](README.md)", "](index.html)" }}
