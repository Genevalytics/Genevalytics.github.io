---
layout: page
title: "Title"
event_date: "2025-04-24"
start_time: "6:00 PM"
end_time: "8:00 PM"
location: "University of Geneva, Room TBD"
speakers:
  - name: "Speaker 1"
    title: "Data Scientist"
    bio: "this is the speaker's bio"
    url: "no-link"
speakers:
  - name: "Speaker 2"
    title: "Data Scientist"
    bio: "this is the speaker's bio"
    url: "no-link"
agenda:
  - time: "6:30 PM - 7:15 PM"
    activity: "Presentation and Q&A"
  - time: "7:15 PM - 9:00 PM"
    activity: "Networking"
contact_email: "contact@genevalytics.ch"
upcoming: false
hide: true
---

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