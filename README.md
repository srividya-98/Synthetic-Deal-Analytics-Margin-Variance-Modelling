# Synthetic-Deal-Analytics-Margin-Variance-Modelling

**📌 Overview**
This project simulates a multi-region commercial “deals” dataset and performs a full margin variance analysis, similar to Big 4 Deal Advisory / commercial analytics work.

**🎯 Objectives**
--To generate synthetic deals with forecast vs actual metrics
--Compute margin deltas and break them into:
**Calcualte**
--Volume variance
--Price variance
--Mix variance
--Fit a DecisionTreeRegressor to quantify margin drivers
--Identify high-risk regions/sectors

**Data Description**
| Column                               | Description                                  |
| ------------------------------------ | -------------------------------------------- |
| `region`                             | APAC/EMEA/Americas                           |
| `sector`                             | Energy, Retail, Tech, Manufacturing, Finance |
| `forecast_volume`, `actual_volume`   | Units                                        |
| `forecast_price`, `actual_price`     | Price per unit                               |
| `forecast_margin`, `actual_margin`   | Margin value                                 |
| `margin_delta`                       | Difference between actual & forecast         |
| `volume_var`, `price_var`, `mix_var` | Variance components                          |



