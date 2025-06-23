---
permalink: /experience/
title: "Experience"
---

{% for exp in site.data.experience %}
## **{{ exp.title }}** 
[{{ exp.company.name }}]({{ exp.company.url }}) - {{ exp.employment.type }}<br>
{{ exp.employment.start }} - {{ exp.employment.end }} | {{ exp.company.location }} ({{ exp.employment.location }})<br>
{% for desc in exp.description %}
- {{ desc }}
{% endfor %}
{% endfor %}
