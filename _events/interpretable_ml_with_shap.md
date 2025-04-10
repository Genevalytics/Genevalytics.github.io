---
layout: page
title: "Interpretable Machine Learning with SHAP Values"
event_date: "2025-04-24"
start_time: "6:15 PM"
end_time: "8:00 PM"
location: "University of Geneva, Uni Mail Room M3220"
speakers:
  - name: "Carson Sprock"
    title: "Data Scientist"
    bio: "Carson is a data scientist from California who has worked in the freight and commodities industries in the United States and Switzerland."
    url: "https://csprock.github.io"
agenda:
  - time: "6:15 PM - 7:00 PM"
    activity: "Presentation and Q&A"
  - time: "7:15 PM - 8:00 PM"
    activity: "Networking"
contact_email: "contact@genevalytics.ch"
upcoming: true
hide: false
series_number: 1
---

Explaining how a model arrived at a prediction is an important part of using machine learning. In this hands-on presentation, we will be exploring how to use [SHAP values](https://proceedings.neurips.cc/paper_files/paper/2017/file/8a20a8621978632d76c43dfd28b67767-Paper.pdf), a widely used model interpretation method, and compare them with other methods. You will learn what SHAP values are and how to apply them using the popular [shap](https://shap.readthedocs.io/en/latest/) Python library. 

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