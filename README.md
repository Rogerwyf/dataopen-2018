# US-311-Service-Requests-and-Food-Establishment-Data-Analysis

[Final Report](https://github.com/Rogerwyf/US-311-Service-Requests-and-Food-Establishment-Data-Analysis/blob/master/FinalReport.pdf)

## Background
U.S 311 Service Requests are requests for non-emergency City services and information. In Citadel & Correlation One The Data Open 2018, we were given a particular dataset containing requests related to food safety and restaurant hygiene volations. We were then asked to come up with our own research question and answer it ourselves.

## Objective
Question: How do governmental actions have influence on health quality of a county or a city?

## Analysis
Step 1. Requests vs Inspections
- Cross referenced by heatmaps (lat,long)
- Ranking of average request processing time, per county by chart
- Ranking of re-inspections that still have violations, per county by chart
- Annoate city locations on the heatmaps (can do if we have time)

Step 2. Regression
- Each record = one county in a period P (e.g 2010-2012)
- Select an appropriate health indicator in P as response
- Feature engineering 
	* Average Pop w/ public insurance / total pop in P
	* Inspections w/ violations / total inspections in P
	* Average time of request processing time (normalized) in P
	* Average income in P
- XGBoost
- GLM
