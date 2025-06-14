---
layout: page
title: "Introduction to Docker, Part 2"
event_date: "2025-06-25"
start_time: "6:30 PM"
end_time: "8:00 PM"
location: "University of Geneva, Uni Mail Room M3220"
address: "Bd du Pont-d'Arve 40, 1205 Genève"
address_url: "https://maps.app.goo.gl/EuSxiVLrYaZ13Gkp9"
speakers:
  - name: "Carson Sprock"
    title: "Data Scientist"
    bio: "Carson is a data scientist from California who has worked in the freight and commodities industries. He is a generalist but has a special interest in time series."
    url: "https://csprock.github.io"
agenda:
  - time: "6:30 PM - 7:15 PM"
    activity: "Presentation and Q&A"
  - time: "7:15 PM - 8:00 PM"
    activity: "Drinks"
contact_email: "contact@genevalytics.ch"
presentation_url: https://github.com/csprock/docker_tutorials
upcoming: true
hide: false
series_number: 5
---

Building on the previous presentation, we will introduce persistent storage in Docker and the difference between bind mounts and volumes and presents examples of each.

### Event Details

- **Date:** {{ page.event_date | date: "%B %d, %Y" }}
- **Time:** {{ page.start_time }} - {{ page.end_time }}
- **Location:** {{ page.location }}
{% if page.presentation_url %}- **[Presentation Material]({{ page.presentation_url }})** {% endif %}

### Speakers

{% for speaker in page.speakers %}
**[{{ speaker.name }}]({{ speaker.url }})**
*{{ speaker.title }}*

{% if speaker.bio %} {{ speaker.bio }} {% endif %}


{% endfor %}

### Agenda

{% for item in page.agenda %}
1. **{{ item.time }}:** {{ item.activity }}
{% endfor %}

---

For any questions about this event, please contact us at [{{ page.contact_email }}](mailto:{{ page.contact_email }}).