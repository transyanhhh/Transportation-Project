# Transportation Project
# Project summary
To continue developing supply-chain analytics skills, I analyzed four years (2021–2024) of transportation performance for a fictional logistics company using the Logistics and Supply Chain dataset (Austin Lasseter). The analysis measures on-time delivery rates, ETA Variation, shipping cost patterns, and impacts of traffic congestion and shipment risk levels. Results are produced at monthly and annual granularity, segmented by shipment status, traffic congestion level, Year/Month, ETA variation (hours) and risk classification, visualized through an interactive Power BI dashboard.  
**Dataset**: [Kaggle - Logistics and Supply Chain Dataset](https://www.kaggle.com/datasets/datasetengineer/logistics-and-supply-chain-dataset/data)
# Objectives & KPIs
**Main Objective:** To analyze the operational efficiency of transportation in shipments over a 4-year period (2021-2024) using KPIs. To identify the causes of increased transportation costs and propose measures to optimize transportation operations.  
**Key KPIs**:
Delay Rate: Number of delayed shipments / total shipments
On-Time Rate: Number of on-time shipments / total shipments
Average ETA (hours): Average difference between estimated arrival time (ETA) and actual arrival time
Transportation Cost Analysis: Based on delivery status, traffic congestion levels, and risk classification
# Key Results
The business is experiencing long-term and systemic shipping delays, not just a minor issue, which increases shipping costs.  
**Delayed Percentage**: 83% of total shipments (only 5,462 on-time shipments out of 32,000), indicating that the majority of orders did not meet the ETA, leading to the risk of SLA violations and significantly impacting customer experience.  
**Delayed shipment cost**: accounts for 83% of total shipping costs. Delayed shipments increase costs due to penalties.  
**Average ETA Variation**: 2.89 hours, indicating that the problem is not an isolated incident but an operational issue (traffic, planning, routing).  
**Traffic Congestion Level**: When congestion is too low (level 0–3), drivers can drive faster, but the route is not optimal (fewer stops at transfer points). When congestion is too high (level 9–10), costs skyrocket due to waiting time, fuel, hourly penalties, and overtime.  
**The ETA deviations by risk** showed no significant differences: High 2,886 hours (33.42%), Medium 2,885 hours (33.3%), Low 2,883 hours (33.28%); indicating that delays are a systemic problem, and the current risk classification is not robust enough to predict or mitigate delivery delays.  
**The recurring cost lows in February** for many years (306K - 311K) suggest that logistics is heavily influenced by seasonality, linked to demand cycles and early year holidays.
# Recommended Actions  
**Optimize traffic routes:** Use traffic congestion level data for route optimization (select routes with levels 5–7 instead of just the shortest or fastest). Use historical data to avoid frequently congested routes, combining it with peak hour forecasting tools to significantly reduce ETA deviations.  
**Manage by risk level:** Increase monitoring and resources for high-risk shipments; balance allocation to improve performance at other risk levels, reducing investment costs in low-risk shipments.  
**Stabilize and control costs:** Apply time series forecasting models to detect seasonal cost peaks early, thereby adjusting operational plans in a timely manner.  
**Cost Control Measures:** Introduce delay penalties in driver incentives tied to ETA adherence and fuel efficiency, targeting the 83% of delayed shipments driving up costs. Track and audit overtime/fuel spikes in heavy congestion (levels 9–10) quarterly to negotiate better carrier terms.
