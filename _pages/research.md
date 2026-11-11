---
layout: page
permalink: /research/
title: research
description: Mathematical biology, infectious disease modeling, optimal control, and forecasting.
nav: true
nav_order: 1
---

My research lies at the intersection of mathematical biology, infectious disease modeling, optimal control, and data-driven forecasting. I aim for models that are mathematically sound, fitted and tested against real data, and useful to people making public health and resource-management decisions.

#### Vaccine hesitancy and disease dynamics

How do attitudes toward vaccination change during an epidemic, and how do those changes shape the epidemic itself? I develop compartmental models with a vaccine-hesitant susceptible class whose hesitancy declines in response to observed deaths, and calibrate them to COVID-19 case, death, vaccination, and survey data from the United States, United Kingdom, South Africa, France, and Brazil. This work forms one part of my dissertation.

#### Sexually transmitted infections

With collaborators, I model syphilis transmission among men who have sex with men, including reinfection, two-stage treatment, and treatment failure ([_Frontiers in Public Health_, 2026](https://doi.org/10.3389/fpubh.2026.1841745)), and behavioral heterogeneity in chlamydia transmission using U.S. surveillance data. Building on these models, I assembled an [open state-level syphilis and chlamydia panel]({{ '/software/' | relative_url }}) for 2000–2024 and used it to score, state by state, how well published transmission models predict years they were not fitted to.

#### Optimal control of multi-species fisheries

Harvesting one species affects its predators and prey. Using Pontryagin's Maximum Principle, I design harvesting strategies for a three-species system in the southern Black Sea (horse mackerel, Atlantic bonito, and bluefish) that balance economic return with the long-term sustainability of each stock ([_Natural Resource Modeling_, 2026](https://doi.org/10.1111/nrm.70044)). This work forms the second part of my dissertation.

#### Forecasting with limited data

I build ensemble forecasting pipelines that combine mechanistic models (SIR-H, SEIR, Bayesian and stochastic SEIR) with statistical models (ARIMA, exponential smoothing, Gaussian processes) and weight them adaptively as data arrive. This approach won the 2026 _Modeling the Invisible_ competition on forecasting viral spread with limited data at Georgia State University.

#### Methods and tools

Ordinary and delay differential equations; optimal control (forward–backward sweep); stability and sensitivity analysis; parameter estimation with multistart optimization; ensemble and probabilistic forecasting. I work mainly in MATLAB, Python, and R.
