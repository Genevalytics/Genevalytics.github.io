---
layout: page
title: "High-Speed Data Analysis in Finance: An Introduction to Polars"
event_date: "2025-05-28"
start_time: "6:15 PM"
end_time: "8:00 PM"
location: "University of Geneva, Uni Mail Room M3220"
address: "Bd du Pont-d'Arve 40, 1205 Genève"
address_url: "https://maps.app.goo.gl/EuSxiVLrYaZ13Gkp9"
presentation_url: 
speakers:
  - name: "Victor Moreno"
    title: "Quantitative Analyst"
    bio: "Skilled in data science and data modelling in Python, Victor is passionate about solving complex mathematical problems."
    url: "https://victor-moreno.com/"
agenda:
  - time: "6:15 PM - 7:00 PM"
    activity: "Presentation and Q&A"
  - time: "7:15 PM - 8:00 PM"
    activity: "Networking and Drinks"
contact_email: "contact@genevalytics.ch"
upcoming: false
hide: false
series_number: 2
---

This talk introduces [Polars](https://pola.rs/), a modern DataFrame library built for speed and efficiency, ideal for high-frequency and large-scale financial data processing.

We'll walk through real-world comparisons between Polars and Pandas using candlestick data (klines), showcasing how Polars handles tasks like loading, parsing, and aggregating massive CSV files with ease.
Attendees will learn how to use LazyFrames, perform datetime conversions, and optimize workflows for time-series analysis.

Live benchmarks and code examples will highlight practical performance gains in common use cases.

Whether you're a quant, analyst, or data engineer, this session will show how Polars can dramatically speed up your data pipelines.

### Event Details

- **Date:** {{ page.event_date | date: "%B %d, %Y" }}
- **Time:** {{ page.start_time }} - {{ page.end_time }}
- **Location:** {{ page.location }}
- **Address:** [{{ page.address }}]( {{ page.address_url }} )
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