# US-311-Service-Requests-and-Food-Establishment-Data-Analysis

Question: How do governmental actions have influence on health quality of a county or a city?

Step 1. Requests vs Inspections
- Cross referenced by heatmaps (lat,long)
- Ranking of average request processing time, per county by chart
- Ranking of re-inspections that still have violations, per county by chart
- Annoate city locations on the heatmaps (can do if we have time)

Step 2. Regression
- Each record = one county in a period P (e.g 2010-2012)
- Select an appropriate health indicator in P as response
- Feature engineering 
	x1. Average Pop w/ public insurance / total pop in P
	x2. inspections w/ violations / total inspections in P
	x3. Average time of request processing time (normalized) in P
	x4. Average income in P
- XGBoost
- GLM
