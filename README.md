# Climate–Tourism Shifts

**Goal:** Quantify how global warming affects international tourism flows, comparing historically-cold countries (e.g. UK, Northern Europe) with already-hot destinations (Mediterranean, Middle East, Africa).

---

## Motivation
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
