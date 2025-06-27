---
layout: page
title: "Introduction to Docker, Part 1"
event_date: "2025-06-18"
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
upcoming: false
hide: false
series_number: 4
---

In the first part of this three part series, we will introduce the containerization paradigm for development and important concepts for understanding Docker. Images, containers and Dockerfiles will be introduced and then we will dive in with basic Docker commands. 

The series will progressively build, ending with building a complete Dockerized application in Python.

## Event Details

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