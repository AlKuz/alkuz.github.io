---
permalink: /experience/
title: "Experience"
---

{% for exp in site.data.experience %}
  <div class="experience-card">
    <div class="exp-header">
      <h3 class="exp-title">{{ exp.title }}</h3>
      <span class="exp-company">
        <a href="{{ exp.company.url }}" target="_blank">{{ exp.company.name }}</a>
      </span>
      <span class="exp-location">{{ exp.company.location }}</span>
    </div>
    <div class="exp-details">
      <span class="exp-dates">
        {{ exp.employment.start }} &ndash; {{ exp.employment.end }}
      </span>
      <span class="exp-type">{{ exp.employment.type }}</span>
      <span class="exp-remote">{{ exp.employment.location }}</span>
    </div>
    <ul class="exp-description">
      {% for item in exp.description %}
        <li>{{ item }}</li>
      {% endfor %}
    </ul>
    <div class="exp-skills">
      {% for skill in exp.skills %}
        <span class="exp-skill">{{ skill }}</span>
      {% endfor %}
    </div>
  </div>
{% endfor %}
