
# VoltRelay Energy - Battery Swapping Network Analytics

## Gradient Data Analytics Hackathon

An end-to-end data analytics project developed for the **Gradient Data Analytics Hackathon**, focused on understanding the operational performance, service quality, profitability, and customer retention of **VoltRelay Energy's battery-swapping network**.

---

## 📌 Project Overview

VoltRelay Energy operates a battery-swapping network for electric two-wheelers (2W) and three-wheelers (3W) across six Indian cities:

- Bengaluru
- Delhi NCR
- Hyderabad
- Pune
- Mumbai
- Jaipur

The network serves gig and logistics riders across segments such as food delivery, quick commerce, e-commerce logistics, cargo, and bike-taxi.

The platform has approximately 18 months of operational history covering swap attempts, station operations, battery lifecycle information, riders, fleet partners, support tickets, pricing, and related operational context.

The objective of this project is to transform this operational data into evidence-based insights that help understand:

- Network performance
- Service failures
- Station and geographic patterns
- Battery and equipment performance
- Pricing and partner economics
- Customer retention and churn
- Revenue and contribution margins

---

## 🎯 Problem Statement

VoltRelay Energy experienced significant growth in completed swaps and revenue, but at the same time faced increasing service failures, changes in rider retention, and pressure on per-swap profitability.

The challenge is to determine:

1. How the network has performed over time.
2. Which factors are associated with service failures and poor customer experience.
3. Where performance differs across stations and cities.
4. How battery health, suppliers, and equipment relate to operational performance.
5. How pricing and fleet partner contracts affect revenue and contribution.
6. Which factors are associated with new riders not returning to the platform.

The analysis focuses on evidence from the available data rather than assumptions.

---

## 🔍 Core Analytical Questions

### 1. Network Performance Over Time

How have the following changed across the available period?

- Completed swaps
- Revenue
- Failure rates
- Contribution margin per swap

The analysis compares these metrics over time to identify whether operational growth is accompanied by changes in service quality and profitability.

---

### 2. Service Failures and Customer Experience

The project investigates how service failures and customer experience vary according to:

- Queue wait time
- Failed attempts
- Abandoned swaps
- Station
- Hour of day
- Vehicle class
- City
- Operational events

This helps identify whether service quality issues are distributed across the network or concentrated in particular operating conditions.

---

### 3. Station and Geographic Patterns

Station-level and city-level analysis is performed to understand differences associated with:

- City
- Station
- Charger generation
- Location type
- Station performance
- Failure rate
- Swap volume
- Revenue
- Contribution

The analysis helps identify stations and geographic areas that require further operational investigation.

---

### 4. Battery and Equipment Performance

Battery and supplier analysis examines:

- Battery state of health
- Delivered battery health
- Charge cycles
- Battery supplier
- Battery pack type
- Delivered range
- Swap frequency
- Energy cost
- Contribution per swap

This helps identify differences between battery suppliers, battery pack types, and equipment cohorts.

---

### 5. Pricing and Partner Economics

The project analyzes the financial impact of:

- Tariff types
- Standard pricing
- Peak pricing
- Off-peak pricing
- Partner pricing
- Discounts
- Energy costs
- Fleet partner contracts
- Partner segments

The analysis compares revenue and contribution across different pricing and partner structures.

---

### 6. Customer Retention

Customer retention is analyzed using:

- Overall retention
- 7-day retention
- 30-day retention
- Cohort retention
- Signup channel
- Vehicle class
- Plan type
- City
- Queue duration
- Failure experience
- Support-ticket exposure
- Tariff type

The goal is to identify factors associated with riders returning to the platform.

> Retention analysis is treated as descriptive/associational analysis. The project does not claim that an observed relationship proves causation.

---

# 📊 Key Analysis Areas

## 1. Operational KPI Analysis

Monthly KPIs include:

- Swap attempts
- Completed swaps
- Revenue
- Completion rate
- Failure rate
- Revenue per completed swap

These metrics provide a high-level view of network performance over time.

---

## 2. City-Level Analysis

Performance is compared across:

- Bengaluru
- Delhi NCR
- Hyderabad
- Pune
- Mumbai
- Jaipur

Metrics include:

- Swap attempts
- Completed swaps
- Revenue
- Completion rate
- Failure rate
- Revenue per completed swap

---

## 3. Vehicle Analysis

The project compares:

- Two-wheelers (2W)
- Three-wheelers (3W)

Key metrics include:

- Swap volume
- Completion rate
- Failure rate
- Revenue
- Revenue per completed swap

---

## 4. Station Performance

Station-level analysis identifies stations with unusual or relatively high service failure rates.

The analysis considers:

- Swap volume
- Completed swaps
- Revenue
- Completion rate
- Failure rate
- Revenue per completed swap
- Station location type
- Charger generation

---

## 5. Failure Analysis

Swap events are categorized into operational outcomes such as:

- Completed swaps
- Failed due to no charged battery
- System errors
- Queue abandonment
- Rider cancellations

Failure analysis is used to understand the main sources of unsuccessful swap experiences.

---

## 6. Revenue and Contribution Analysis

Financial analysis includes:

- Revenue
- Discounts
- Energy costs
- Direct contribution
- Contribution per completed swap
- Revenue per swap

Monthly contribution analysis is also used to understand changes in financial performance over time.

---

## 7. Supplier Analysis

Battery suppliers are compared using:

- Completed swaps
- Revenue
- Energy cost
- Contribution
- Battery state of health
- Delivered battery health
- Average range
- Contribution per swap

---

## 8. Battery Pack Analysis

Different battery pack configurations are compared based on:

- Completed swaps
- Revenue
- Energy cost
- Contribution
- State of health
- Average range
- Contribution per swap

---

## 9. Fleet Partner Analysis

Fleet partners are analyzed using:

- Completed swaps
- Revenue
- Discounts
- Energy cost
- Contribution
- Partner segment
- Contract type
- Discount percentage

Partner segments include categories such as:

- Food delivery
- Quick commerce
- E-commerce logistics
- Bike taxi
- Cargo / 3W

---

## 10. Customer Retention Analysis

Retention analysis includes:

### Overall Retention

- 7-day retention
- 30-day retention

### Cohort Retention

Riders are grouped according to their signup period to examine retention across cohorts.

### Retention by Channel

- App store
- Field agent
- Partner onboarding
- Referral

### Retention by Vehicle

- 2W
- 3W

### Retention by Queue Experience

Retention is compared across different queue-duration groups.

### Retention by Other Factors

- City
- Plan type
- Tariff
- Failure experience
- Support-ticket exposure

---

# 📈 Visualizations

The repository contains generated visualizations covering major analytical areas.

Examples include:

- Network Reliability Trend
- Monthly Failure Rate
- Monthly Revenue and Failure Rate
- Revenue per Completed Swap Over Time
- Failure Rate by City
- Failure Rate by Vehicle Class
- Failure Rate by Hour of Day
- Top 10 Stations by Failure Rate
- Overall Swap Event Distribution
- Swap Attempt Outcome Distribution
- Technical Failure Reasons
- Retention Rate by Queue Duration
- Direct Contribution per Completed Swap
- Direct Contribution per Swap by Fleet Partner
- Average Delivered Battery Health by Supplier
- Average Distance Since Previous Swap
- Demand and Service Pressure by Hour

All generated charts are available in the `Output/` directory.

---

# 🛠️ Technologies Used

- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Seaborn**
- **Google Colab**
- **Jupyter Notebook**

---

# 📂 Project Structure

```text
VoltRelay-Battery-Swapping-Analytics/
│
├── data/
│   └── README.md
│
├── Output/
│   ├── Avg Delivered Battery Health by Supplier.png
│   ├── Avg Distance Since Previous Swap.png
│   ├── Completed Battery Swap Increased Strongly.png
│   ├── Demand and Service Pressure by Hour.png
│   ├── Direct Contribution per Completed Swap.png
│   ├── Direct Contribution per Swap by Fleet Partner.png
│   ├── Failure Rate by City.png
│   ├── Failure Rate by Hour of Day.png
│   ├── Failure Rate by Vehicle Class.png
│   ├── Monthly Failure Rate.png
│   ├── Monthly Revenue and Failure Rate.png
│   ├── Network Reliability Trend.png
│   ├── Overall Swap Event Distribution.png
│   ├── Retention Rate by Queue Duration.png
│   ├── Revenue Per Completed Swap Over Time.png
│   ├── Service Failure Rate by City.png
│   ├── Service Failure Rate by Vehicle Class.png
│   ├── Swap Attempt Outcome Distribution.png
│   ├── Technical Failure Reasons.png
│   └── Top 10 Stations by Failure Rate.png
│
├── VoltRelay_Energy_Battery_Swapping_Network_Analytics.ipynb
├── requirements.txt
└── README.md
```
