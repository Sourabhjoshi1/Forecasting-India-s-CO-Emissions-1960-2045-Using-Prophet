
# Forecasting India's CO₂ Emissions (1960–2045) Using Facebook Prophet

This notebook demonstrates how to use Facebook's [Prophet](https://facebook.github.io/prophet/) model to forecast India's CO₂ emissions over the next 30 years based on historical data from 1960 to 2019.

---

### Objective

- Understand India's historical carbon emission trends
- Use time-series forecasting (Prophet) to predict future CO₂ emissions
- Visualize and interpret results for climate awareness and policy insights

---

###  Dataset

- **Source**: [Our World in Data – CO₂ Emissions](https://ourworldindata.org/co2-emissions)
- **Time Period Used**: 1960 to 2019
- **Columns Used**:
  - `Entity` → renamed to `country`
  - `Annual CO₂ emissions (tonnes )` → renamed to `co2`
  - `Year` → renamed to `ds` for Prophet compatibility
- **Filtered**: Only India, and years from 1960 onwards

---

###  Model: Facebook Prophet

- Prophet is robust to missing data and trend changes.
- Automatically detects trend shifts and forecasts with uncertainty intervals.
- Excellent for time series like this with long-term growth.

---

###  Forecast Overview

- Trained the model on CO₂ emissions data from 1960–2019
- Forecasted emissions from 2020 to 2045
- Confidence intervals (yhat_lower, yhat_upper) included for uncertainty

---

###  Key Insights

- India's emissions were low until 1980, after which exponential growth began.
- The model projects continued growth in CO₂ emissions if trends remain unchanged.
- **Forecast for 2030**: Approximately 3.1 billion tonnes of CO₂ (± confidence margin).
- This highlights the **urgency of sustainable development and clean energy adoption**.

---

### Conclusion

India’s CO₂ emissions are on a sharply rising trajectory and are projected to exceed 3.1 billion tonnes by 2030, if current trends continue.
Using Facebook Prophet, a time-series model, we captured the long-term trend in emissions growth since 1960 and forecasted it up to 2045.
The model’s results reinforce the urgency for sustainable energy transitions and policy interventions to mitigate future environmental impact.

---

### Future Work

- Compare results with ARIMA, LSTM, or other deep learning models.
- Explore forecasting for other countries or per capita emissions.
- While Prophet handled the trend well, integrating external factors like GDP, energy mix, and industrial growth could enhance prediction accuracy — a potential direction for future work.

---

 Developed by Sourabh Joshi : M.Tech in Power Electronics & Drives, passionate about clean energy, data science, and global impact.
