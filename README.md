# 🚕 Revenue Maximization for Taxi Drivers — Payment Type Analysis

## Overview
This project investigates whether payment method (card vs cash) has a statistically
significant impact on taxi fare amounts, using NYC Taxi Trip records.
The goal: identify data-driven strategies to maximize driver revenue without
compromising customer experience.

---

## Problem Statement
Can nudging customers toward card payments generate higher revenue for drivers?

---

## Dataset
- Source: NYC Taxi Trip Records
- Key columns used: `passenger_count`, `payment_type`, `fare_amount`,
  `trip_distance`, `duration`

---

## Methodology
| Step | Description |
|------|-------------|
| Descriptive Analysis | Summary stats on fare amount and payment type distribution |
| Hypothesis Testing | T-test comparing average fares across payment methods |
| Regression Analysis | Linear regression of trip duration vs fare amount |

---

## Key Findings

<img width="1160" height="622" alt="image" src="https://github.com/user-attachments/assets/638eedf9-aca1-44f9-8816-5ce028eb349e" />

- Card payments account for **67.5%** of all transactions
- Card avg fare: **$13.70** vs Cash avg fare: **$12.25** (~11.8% higher)
<img width="1050" height="592" alt="image" src="https://github.com/user-attachments/assets/c9bd7510-4474-4617-b082-2ec2fe96460f" />

- Card avg trip distance: **3.23 miles** vs Cash: **2.80 miles**
- T-statistic: **165.5**, p-value **< 0.05** → reject null hypothesis
- Single-passenger rides dominate both payment types (40% card, 20% cash)

---

## Conclusion
There is a statistically significant difference in fare amounts between card
and cash payments. Encouraging card adoption can meaningfully improve
driver revenue.

---

## Recommendations
- Offer incentives or discounts for card transactions
- Ensure seamless, secure card payment UX at booking
- Target single-passenger rides for card nudge campaigns

---

## Tech Stack
`Python` · `Pandas` · `SciPy` · `Matplotlib` · `Seaborn`
