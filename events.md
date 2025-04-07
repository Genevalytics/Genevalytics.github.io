---
layout: page
title: Events
---

## Upcoming Events

{% assign sorted_events = site.events | sort: "series_number" %}

{% for event in sorted_events %}
  {% if event.upcoming and event.hide != true %}
### [{{ event.title }}]({{ event.url }})
**Date:** {{ event.event_date | date: "%B %d, %Y" }}
**Time:** {{ event.start_time }} <br>
**Location:** {{ event.location }}

[More information]({{ event.url }})

---
  {% endif %}
{% endfor %}

{% unless site.events | where: "upcoming", true | where_exp: "item", "item.hide != true" %}
No upcoming events scheduled. Check back soon!
{% endunless %}

## Past Events

{% for event in sorted_events reversed %}
  {% unless event.upcoming or event.hide == true %}
### [{{ event.title }}]({{ event.url }})
**Date:** {{ event.event_date | date: "%B %d, %Y" }}  
**Location:** {{ event.location }}

[More information]({{ event.url }})

---
  {% endunless %}
{% endfor %}

{% unless site.events | where_exp: "item", "item.upcoming != true and item.hide != true" %}
No past events yet.
{% endunless %}