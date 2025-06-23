---
permalink: /experience/
title: "Experience"
---

{% for exp in site.data.experience %}
## **{{ exp.title }}** 

🏢 {% if exp.company_url != "null" %}
[{{ exp.company_name }}]({{ exp.company_url }}) - {{ exp.employment_type }}
{% else %}
{{ exp.company_name }} - {{ exp.employment_type }}
{% endif %}

📍 {{ exp.company_location }} - {{ exp.employment_location }}

🕓 {{ exp.employment_start }} - {{ exp.employment_end }}

{% for desc in exp.description %}
- {{ desc }}
{% endfor %}
{% endfor %}
