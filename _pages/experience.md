---
permalink: /experience/
title: "Experience"
---

{% set dot_separator = ' · ' %}

{% for exp in site.data.experience %}
## **{{ exp.title }}** 
🏢 {% if exp.company_url != "null" %}
[{{ exp.company_name }}]({{ exp.company_url }})
{% else %}
{{ exp.company_name }}
{% endif %}
[{{ exp.company_name }}]({{ exp.company_url }}) - {{ exp.employment_type }}<br>
📍 {{ exp.company_location }} - {{ exp.employment_location }}<br>
🕓 {{ exp.employment_start }} - {{ exp.employment_end }}<br>
✅ {{ exp.skills | join(dot_separator) }}
{% for desc in exp.description %}
- {{ desc }}
{% endfor %}
{% endfor %}
