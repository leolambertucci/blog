---
title: Trem de infra
---
Terraform, Ansible, DevOps, Iac, SRE, Monitoring, Scripts, Python

{% for tag in site.tags %}
  Name: {{ tag | first }},
  count: {{ tag | last | size}}
{% endfor %}
