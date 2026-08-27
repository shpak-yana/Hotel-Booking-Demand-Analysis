# 🏨 Hotel Booking Demand Analysis

An end-to-end exploratory data analysis (EDA) project examining hotel booking patterns, cancellation behaviours, and guest demographics. The goal was to translate raw data into actionable business insights for revenue management and marketing optimisation.

## 📌 Project Overview

This project analyses a publicly available hotel booking dataset containing **~120,000 records** from both **City Hotels** and **Resort Hotels**. Using Python and core data analysis libraries, I investigated seasonal demand trends, geographical booking distributions, and the impact of family composition on cancellation rates.

By treating this as a real-world business case, I aimed to answer the following questions:

- Which countries generate the most successful bookings?
- How does the length of stay differ between hotel types?
- How often do guests receive a different room type than they reserved (overbooking proxy)?
- When are the busiest booking months, and how does seasonality affect cancellations?
- Do families with children behave differently in terms of booking stability (churn)?

## 🔍 Key Analyses Performed

1. **Data Cleaning & Preprocessing** – Standardised column names, handled missing values in `country` and `children`, and checked for duplicates.
2. **Geographic Analysis** – Identified the top 5 countries contributing to successful hotel stays.
3. **Stay Duration** – Calculated average nights per booking for City vs. Resort hotels.
4. **Room Type Mismatch** – Quantified instances where the assigned room differed from the reserved room (a key indicator of overbooking).
5. **Seasonality & Cancellation Trends** – Mapped the most popular booking months (2016 vs. 2017) and isolated peak cancellation months for City Hotels.
6. **Guest Demographics** – Analysed the average distribution of adults, children, and babies per booking.
7. **Family Impact** – Engineered a `has_kids` flag to measure how families influence the **churn rate** (cancellation percentage).

## 📊 Key Insights & Business Recommendations

- **Top Source Markets**: Portugal (PRT) and the United Kingdom (GBR) are the dominant source markets, presenting a clear target for loyalty programmes and regional marketing spend.
- **Cancellation Risk**: The **churn (cancellation) rate is consistently higher for bookings involving children**. Families are more likely to cancel than adult-only groups. *Recommendation: Introduce family-friendly flexible cancellation policies or early-bird discounts to secure these bookings.*
- **City Hotel Seasonality**: Cancellations for City Hotels peak sharply during **specific months** (e.g., early Autumn) – a strong signal for adjusting overbooking thresholds and staff allocation.
- **Overbooking Occurrence**: A non-trivial percentage of bookings receive a different room type. This suggests operational overbooking is prevalent and should be monitored to prevent guest dissatisfaction.
- **Stay Preferences**: Resort Hotel stays are, on average, longer than City Hotel stays, indicating leisure vs. business travel segmentation.

## 🛠️ Tech Stack

- **Python 3** – Core programming language.
- **Pandas** – Data manipulation and cleaning.
- **Matplotlib / Seaborn** – Data visualisation (bar charts, heatmaps).
- **Jupyter Notebook** – Interactive development environment.

## 🚀 How to Run the Project

1. Clone this repository to your local machine.
2. Ensure the dataset (`2_bookings.csv`) is placed in the root directory.
3. Install the required dependencies:

```bash
pip install pandas matplotlib seaborn
```

4. Run the analysis script or open the Jupyter Notebook:

```bash
jupyter notebook hotel_booking_analysis.ipynb
```
