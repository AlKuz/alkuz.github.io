---
permalink: /experience/
title: "Experience"
---

{% for exp in site.data.experience %}
## **{{ exp.title }}** 

🏢 {% if exp.company_url != "null" %}
[{{ exp.company_name }}]({{ exp.company_url }})
{% else %}
{{ exp.company_name }}
{% endif %}
[{{ exp.company_name }}]({{ exp.company_url }}) - {{ exp.employment_type }}

📍 {{ exp.company_location }} - {{ exp.employment_location }}

🕓 {{ exp.employment_start }} - {{ exp.employment_end }}

🔧 {% for skill in exp.skills %}
{{ skill }}{% unless forloop.last %} <span style="color: #999;">•</span>{% endunless %}
{% endfor %}

{% for desc in exp.description %}
- {{ desc }}
{% endfor %}
{% endfor %}
