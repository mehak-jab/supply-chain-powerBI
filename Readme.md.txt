# Supply Chain Logistics Risk Analysis (Power BI)

![Dashboard](images/overview.png)

## Business question
What drives high-risk shipments, and do delays, cost or operations differ by risk level?

## Dataset
32,065 hourly logistics records (Jan 2021 – Aug 2024) with GPS, traffic, weather, warehouse,
supplier, driver and risk fields. Source: [dataset name and link, e.g. Kaggle URL]

## Key findings
- Risk class is determined entirely by the disruption likelihood score (above 0.7 = High Risk).
- Traffic, weather, route, driver and supplier factors have no measurable effect on risk.
- Delay probability (~70%) and shipping cost (~$459) are flat across risk classes and over time.
- Only 23.5% of deliveries arrive within 1 hour of plan.

**Recommendation:** review how the disruption score is calculated, since operational
factors are not reflected in the risk classification.

## What I built
- Power Query: type cleanup, calculated band columns (traffic, delay, disruption score)
- Data model: Date table marked as date table, one-to-many relationship, sort-by-column
- DAX measures: On-Time %, High Risk %, % of Total (ALLSELECTED), High Risk Lift by factor,
  Cost MoM % (DATEADD), KEEPFILTERS for slicer-aware measures
- Visuals: KPI cards, Key influencers, stacked column, scatter, matrix, synced slicers

## Example DAX
​```DAX
High Risk % = DIVIDE(CALCULATE([Shipments], KEEPFILTERS(Logistics[risk_classification] = "High Risk")), [Shipments])
​```

## How to open
Download `SupplyChainLogistics.pbix` and open it in Power BI Desktop (free).