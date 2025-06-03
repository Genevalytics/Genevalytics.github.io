---
layout: page
title: "Introduction to Linear Optimization with Python"
event_date: "2025-06-11"
start_time: "6:15 PM"
end_time: "8:00 PM"
location: "University of Geneva, Uni Mail Room M3220"
address: "Bd du Pont-d'Arve 40, 1205 Genève"
speakers:
  - name: "Carson Sprock"
    title: "Data Scientist"
    bio: "Carson is a data scientist from California who has worked in the freight and commodities industries. He is a generalist but has a special interest in time series."
    url: "https://csprock.github.io"
# agenda:
#   - time: "6:30 PM - 7:15 PM"
#     activity: "Presentation and Q&A"
#   - time: "7:15 PM - 9:00 PM"
#     activity: "Networking"
contact_email: "contact@genevalytics.org"
presentation_url: https://github.com/csprock/linear_optimization_with_python
upcoming: true
hide: false
series_number: 3
---

Linear programming is an important tool in the data scientist's toolbelt. In this presentation, we will use an example from the petroleum industry to introduce linear programming, demonstrating the important components of a linear model, how to set up your model, how to take a non-linear problem and convert it into a linear one, and how to use binary decision variables. We will be using the [pyomo](https://www.pyomo.org/) Python library. 


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