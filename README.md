# 🏥 Primary Care Demand Forecasting & Stress Early Warning System

---

## 📌 Overview

This project builds a regional primary care demand forecasting and stress monitoring framework using real NHS General Practice appointment data.

It evaluates how service pressure evolves under:

📈 Seasonal demand growth  
⚠️ Winter pressure spikes  
🏥 Capacity adjustments  
📊 Regional variability  

The system combines forecasting, interpretable stress indexing, and multi-scenario simulation to support operational planning and resilience analysis.

---

## 📊 National Demand Trend

![National Demand Trend](visuals/national_trend.png)

The time-series shows strong seasonal patterns with recurring winter peaks across regions.

---

## 📈 Forecasting Performance (London Example)

![SARIMA Forecast](visuals/sarima_forecast_London.png)

### 🔬 Key Result

| Model | MAE |
|--------|--------|
| Naïve | 345k |
| SARIMA | **205k** |

✅ ~40% reduction in forecasting error  
✅ Successfully captures winter demand spikes  

---

## 🧮 Primary Care Stress Index (PCSI)

\[
PCSI =
Z(\text{Demand Growth}) +
Z(\text{Same-Day %}) +
Z(\text{Demand Volatility})
\]

- 📈 Growth → Pressure increase  
- ⚡ Same-day % → Urgent load  
- 📊 Volatility → Instability  

---

## 🔥 National Stress Heatmap

![PCSI Heatmap](visuals/pcsi_heatmap.png)

Clear synchronised winter stress bands appear across all regions, with London exhibiting the highest peak intensity.

---

## 🔬 Scenario Simulation (London)

### Combined Scenario Comparison

![London Multi Scenario](visuals/simulation/pcsi_multi_scenario_London.png)

### Observations

- 📈 +8% Winter Surge increases stress sharply  
- 📉 +10% Capacity significantly reduces stress  
- ✅ Surge +10% Capacity offsets winter spike  

---

## 📊 National Scenario Impact

### Winter Surge Impact by Region

![Winter Surge Impact](visuals/simulation/national_winter_surge_impact.png)

- 🔴 London most surge-sensitive  
- 🟡 South West least sensitive  

---

### +10% Capacity Benefit by Region

![Capacity Benefit](visuals/simulation/national_capacity_10pct_impact.png)

- 🟢 North East & Yorkshire most responsive  
- 📊 Capacity elasticity varies regionally  

---

## 📊 Scenario Summary Matrix

Exported file:

