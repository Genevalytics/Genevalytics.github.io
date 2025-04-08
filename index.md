---
title: Welcome to Genevalytics
#feature_image: assets/files/banner2.webp
#feature_text: |
#  ## Genevalytics
---


We are excited to announce the launch of Genevalytics, a new speaker series in Geneva for professionals and beginners alike to learn and share knowledge about the latest methods, techniques, technologies and applications of statistics, machine learning and AI. Our goal is to organize practical, hands-on presentations and demonstrations on a semi-regular basis. 

Interested in learning more, contributing to the organization, or giving a talk? Please contact us! 

---

## Announcements

{% assign sorted_announcements = site.announcements | sort: "annoucement_date" | reverse %}
{% assign announcement_upcoming = false %}

{% for announcement in sorted_announcements %}
  {% if announcement.hide != true %}
    {% assign announcement_upcoming = true %}
### [{{ announcement.title }}]({{ announcement.url }})
**Date:** {{ announcement.annoucement_date | date: "%B %d, %Y" }}  



  {% endif %}
{% endfor %}

{% if announcement_upcoming != true %}
*No new announcements. Check back soon!*
{% endif %}

---

## Upcoming Events

{% assign sorted_events = site.events | sort: "series_number" %}
{% assign has_upcoming = false %}

{% for event in sorted_events %}
  {% if event.upcoming and event.hide != true %}
    {% assign has_upcoming = true %}
### [{{ event.title }}]({{ event.url }})
**Date:** {{ event.event_date | date: "%B %d, %Y" }}  
**Time:** {{ event.start_time }} <br>
**Location:** {{ event.location }}

  {% endif %}

{% endfor %}

{% if has_upcoming != true %}
*No upcoming events scheduled. Check back soon!*
{% endif %}

[View all events](/events/)

---


## Partners

We work in conjunction with [WeData](https://wedata.ch/), an association of the University of Geneva that aims to share its passion for data science and computer science. 

![WeData Logo](/assets/files/wedata_logo.png){: .partner-logo}


## Join Our Community

Stay informed about upcoming events by following us:

- [Follow us on LinkedIn](https://www.linkedin.com/company/genevalytics/)
- [Join our WhatsApp group](https://chat.whatsapp.com/Htx3lgNLKeP9TvybQhimct)

## Contact

Have a question or interested in presenting? 

Email us at [contact@genevalytics.ch](mailto:contact@genevalytics.ch)