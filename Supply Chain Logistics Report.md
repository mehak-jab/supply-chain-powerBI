# Supply Chain Logistics Report

dynamic_supply_chain_logistics_dataset.csv · 32,065 hourly records · Jan 2021 – Aug 2024

Year

Risk classification

Traffic congestion

Weather severity

## Executive Overview

### Average delay probability by month

Mean of delay_probability across all hourly records in the month

### Delivery status

Early: deviation \< 0 h · On time: 0–1 h · Late: > 1 h

### Risk classification mix by quarter

Share of records in each risk class (100% stacked)

### Average shipping cost by risk class

Mean of shipping_costs

## Risk & Disruption

### Key influencers: what makes a record High Risk?

High Risk rate when the factor is in its top 25% of values, divided by the overall High Risk rate

### Risk class by disruption likelihood score

Records per 0.1 band of disruption_likelihood_score, stacked by risk class

### Disruption likelihood vs delay probability

Random sample of up to 1,500 filtered records

### Risk class summary

Matrix visual · averages per class

## Operations & Fleet

### GPS hotspot grid: average delay probability

Vehicle positions binned into 2.5° × 5° cells, latitude 30–50°N, longitude 120–70°W

### Driver & fleet scores

Averages on a 0–1 scale

### Traffic congestion by weekday and hour

Average traffic_congestion_level (0–10)

### Fuel consumption by traffic level

Average fuel_consumption_rate per traffic level (rounded down)

## Warehouse & Supply

### Average warehouse inventory level by month

Units on hand (0–1,000)

### Average historical demand by month

Units demanded (100–10,000)

### Lead time by supplier reliability

Average lead_time_days per reliability band

### IoT cargo temperature distribution

Records per 5 °C band

### Loading time by equipment availability

Average loading_unloading_time (hours)