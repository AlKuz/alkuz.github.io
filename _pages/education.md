---
layout: single
permalink: /education/
title: "Education"
author_profile: true
---

# Academic Qualifications

- 2016-2020 [Samara State Aerospace University](https://ssau.ru/english)
  - **Degree:** Candidate of Technical Sciences
  - **Field of study:** Thermal, electric propulsion engines and power plants of aircraft


- 2009-2015 [Samara State Aerospace University](https://ssau.ru/english)
  - **Degree:** Diploma in engineering
  - **Field of study:** Engineer of rocket engines

# Certifications
[<img src="https://images.credly.com/size/680x680/images/778bde6c-ad1c-4312-ac33-2fa40d50a147/image.png" width="170" height="170" alt="Certification Badge: AWS Certified Machine Learning – Specialty">](https://www.credly.com/badges/5a89e256-c9cb-406d-807a-f92196f588b9/public_url)
[<img src="https://images.credly.com/size/680x680/images/a253b994-caa6-4dd1-bf0e-434dd012b1f6/image.png" width="170" height="170" alt="Certification Badge: AWS Partner: Technical Accredited">](https://www.credly.com/badges/795e9bdb-affe-4022-bfab-c92b4561a2bb/public_url)
[<img src="https://images.credly.com/size/680x680/images/145a5de8-7390-4d57-b4cb-a10e2f9394e2/image.png" width="170" height="170" alt="Certification Badge: AWS Partner: Generative AI Essentials">](https://www.credly.com/badges/952d6682-5efe-40f8-a376-04f42d3de04d/public_url)

# Courses
{% for course in site.data.courses %}
- {{ course.date }} - {{ course.platform }} - [{{ course.title }}]({{ course.url }})
{% endfor %}
