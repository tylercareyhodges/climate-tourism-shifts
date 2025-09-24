# Climate–Tourism Shifts

**Goal:** Quantify how global warming affects international tourism flows, comparing historically-cold countries (e.g. UK, Northern Europe) with already-hot destinations (Mediterranean, Middle East, Africa).

---

## Motivation

What originally triggered me to start this project is the amount of heatwaves and the duration we've been having in the UK this year (it's been great)! I was thinking If I were somebody possibly from Europe like Spain, France etc. my want to come to the UK would increase given that the UK is having better summers now (on average - or at least will have "better" summers on average in the future on average). I thought it would be a good idea to create a data pipeline to see if the trends in tourism due to global warming were already a factor - although obviously there are far many factors at play! Although, this data pipeline will still be use-able for the foreseable future when we have access to more global warming data and maybe when some countries which rely on tourism become unattractive because they become "too hot" in some parts of the year.

Tourism is one of the world’s largest industries. Climate change is shifting temperature patterns and human comfort zones:
- Historically-cold countries may become *more* attractive as summers warm.
- Already-hot countries risk becoming *too hot*, reducing tourist arrivals.

This project builds a data science pipeline to measure and forecast these effects using international tourism data and climate datasets.

---

## Research questions
1. To what extent does rising temperature increase arrivals to colder countries?  
2. To what extent does excessive heat reduce arrivals to already-hot countries?  
3. Can we project future tourism trends (2030–2050) under climate scenarios (SSP2-4.5, SSP5-8.5)?

---

## Data sources
- **Tourism:** World Bank (international tourist arrivals), UN Tourism, Eurostat.  
- **Climate:** NASA GISTEMP anomalies, ERA5-HEAT (UTCI comfort & heat-stress days), WorldClim CMIP6 scenarios.  
- **Controls:** GDP per capita, exchange rates, population, pandemic dummies.

---

## Methods
- Panel fixed-effects regression (country + year FE).  
- Non-linear temperature and heat-stress thresholds (UTCI).  
- Event-study around extreme-heat summers.  
- Forecasting with ML (XGBoost) and climate scenario forcing.  

---

## Repo layout
