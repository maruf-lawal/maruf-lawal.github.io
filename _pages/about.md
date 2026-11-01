---
permalink: /
title: ""
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

I am a Ph.D. candidate in Mathematics at the **University of Tennessee, Knoxville**, advised by Prof. Suzanne Lenhart, with my degree expected in December 2026. I build mathematical models of infectious disease and ecological systems and use **optimal control**, **parameter estimation**, and **forecasting** to turn them into tools that support decisions in **public health** and **natural resource management**.

My recent work includes compartmental models of vaccine hesitancy and syphilis transmission, an optimal control framework for multi-species fisheries in the Black Sea, an ensemble forecasting approach that won the 2026 *Modeling the Invisible* forecasting competition, and an open state-level surveillance panel for benchmarking STI transmission models.

## Research Interests

- **Infectious disease modeling:** transmission dynamics, behavioral responses and vaccine hesitancy, sexually transmitted infections, model calibration and validation against surveillance data
- **Optimal control and decision science:** intervention design for epidemics; sustainable harvesting of renewable resources
- **Forecasting and data-driven modeling:** ensemble forecasts that combine mechanistic and statistical models, uncertainty quantification
- **Ecological and fisheries modeling:** multi-species predator–prey systems and ecosystem-based management

More on the [Research](/research/) page.

## Recent News

<ul class="news-list">
{% for n in site.data.news limit: 6 %}
  <li><span class="news-date">{{ n.date }}</span> {{ n.text | markdownify | remove: '<p>' | remove: '</p>' }}</li>
{% endfor %}
</ul>
