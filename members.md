---
layout: page
title: Members
---




{% for member in site.members %}
### {{ member.name }}
**{{ member.position }}**

{{ member.content }}

{% if member.website %}[Website]({{ member.website }}){% endif %}{% if member.email %} • [Email](mailto:{{ member.email }}){% endif %}{% if member.linkedin %} • [LinkedIn]({{ member.linkedin }}){% endif %}{% if member.github %} • [GitHub]({{ member.github }}){% endif %}


---
{% endfor %}