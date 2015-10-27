---
---

# States of public repositories

{% for repository in site.github.public_repositories %}
* [{{ repository.name }}]({{ repository.html_url }}) - {{ repository.description }}<br />
  [![Build Status](https://img.shields.io/travis/{{ repository.full_name }}.svg)](https://travis-ci.org/{{ repository.full_name }}.apt)
  [![Issues](https://img.shields.io/github/issues/{{ repository.full_name }}.apt.svg)]({{ repository.issues_url }})
  [![Tag](https://img.shields.io/github/tag/{{ repository.full_name }}.svg)]({{ repository.tags_url }})
{% endfor %}
