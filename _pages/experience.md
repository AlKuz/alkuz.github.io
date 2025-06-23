---
permalink: /experience/
title: "Experience"
---

{% for exp in site.data.experience %}
## **{{ exp.title }}** 
🏢 [{{ exp.company_name }}]({{ exp.company_url }}) - {{ exp.employment_type }}<br>
📍 {{ exp.company_location }} - {{ exp.employment_location }}<br>
🕓 {{ exp.employment_start }} - {{ exp.employment_end }}<br>
{% for desc in exp.description %}
- {{ desc }}
{% endfor %}
{% endfor %}
