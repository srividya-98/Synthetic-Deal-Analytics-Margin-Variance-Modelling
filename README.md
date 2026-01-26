# Synthetic Deal Analytics – Margin Variance Modelling

## Overview
This project simulates a commercial deals dataset and analyses why actual margins differ from forecasted margins.

The focus is on understanding *what changed and why*, rather than just reporting final numbers. The analysis follows the kind of margin variance work commonly done in commercial analytics and deal advisory teams.

---

## What this project does
- Creates a synthetic deals dataset across multiple regions and sectors  
- Compares forecast vs actual volume, price, and margin  
- Breaks margin differences into clear components:
  - volume impact
  - price impact
  - mix impact  
- Uses a decision tree to understand which factors are most often linked to margin changes  
- Highlights regions and sectors that tend to show higher downside risk  

---

## Why this problem matters
In real commercial settings, teams often see that margins missed forecasts but struggle to explain *why*.

A single margin number is not useful on its own. What matters is knowing:
- whether the issue came from volume, price, or mix
- whether the problem is isolated or systematic
- which regions or sectors need attention

This project shows how margin variance analysis can be structured in a clear and explainable way.

---

## Data Description
Each row represents one simulated deal.

| Column | Description |
|------|-------------|
| region | Deal region (APAC, EMEA, Americas) |
| sector | Sector (Energy, Retail, Tech, Manufacturing, Finance) |
| forecast_volume | Expected deal volume |
| actual_volume | Delivered volume |
| forecast_price | Expected unit price |
| actual_price | Realised unit price |
| forecast_margin | Expected margin |
| actual_margin | Realised margin |
| margin_delta | Actual margin minus forecast margin |
| volume_var | Margin impact due to volume change |
| price_var | Margin impact due to price change |
| mix_var | Margin impact due to deal mix |

The dataset is synthetic but structured to resemble real commercial reporting data.

---

## How the analysis works

### 1. Creating synthetic deals
The dataset is generated with controlled variation across regions, sectors, volumes, and prices. 

---

### 3. Breaking margin differences into components
The margin difference is split into:
- volume variance: impact from selling more or fewer units  
- price variance: impact from changes in realised price  
- mix variance: impact from shifts in region or sector composition  


---

### 4. Understanding margin drivers
A decision tree model is used with region, sector, and variance components as inputs.

The purpose of the model is to see which factors are most often associated with higher or lower margins. The model structure makes it easy to spot patterns, such as certain regions or sectors consistently appearing in negative margin outcomes.

---

### 5. Identifying risk areas

---

## Outputs
- Deal-level margin deltas  
- Volume, price, and mix variance components  
- Aggregated views by region and sector  
- Model-based insights into margin drivers  


---

## Possible next steps
- Add stress scenarios for adverse pricing or volume changes  
- Track margin behaviour over time instead of at deal level  
- Build a simple dashboard for regional performance review  
- Compare different modelling approaches for driver analysis  
