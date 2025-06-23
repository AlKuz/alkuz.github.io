---
permalink: /experience/
title: "Experience"
---

{% for exp in site.data.experience %}
## **{{ exp.title }}** 
[{{ exp.company_name }}]({{ exp.company_url }}) - {{ exp.employment_type }}<br>
{{ exp.employment_start }} - {{ exp.employment_end }} | {{ exp.company_location }} ({{ exp.employment_location }})<br>
{% for desc in exp.description %}
- {{ desc }}
{% endfor %}
{% endfor %}
