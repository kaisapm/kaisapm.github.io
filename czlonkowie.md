
---
layout: page
title: Członkowie
---

# Nasi członkowie

Tutaj znajdziesz informacje o członkach naszej drużyny.

{% for member in site.data.members %}
  ## {{ member.name }} ({{ member.handle }})

  <p>{{ member.description }}</p>

  <strong>Umiejętności:</strong>
  <ul>
    {% for skill in member.skills %}
      <li>{{ skill }}</li>
    {% endfor %}
  </ul>
{% endfor %}

