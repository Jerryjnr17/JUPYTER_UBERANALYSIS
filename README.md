Uber Ride Demand & Supply Analysis
Overview

This project analyzes Uber ride data to understand demand–supply dynamics, cancellation drivers, revenue patterns, and the impact of weather conditions. The objective is to derive actionable insights that can support operational planning, pricing strategies, and driver allocation decisions.

Objective

Analyze peak demand periods and supply shortages

Identify key reasons behind ride cancellations and “No Cars Available” events

Evaluate revenue contribution by ride type

Measure the effect of weather on ride fulfillment

Dataset

Total Records: ~6,945 Uber ride requests

Total Features: 13

Key fields include request/start/drop timestamps, pickup and drop locations, ride type, trip cost, tip amount, payment method, driver ID, trip status, and weather conditions.

Data Cleaning & Preprocessing

Converted timestamp fields into datetime format

Engineered new features:

Request hour and day of week

Wait time (start time − request time)

Trip duration (drop time − start time)

Standardized pickup and drop location names

Identified that all cancelled and “No Cars Available” trips lack start and drop times

Retained these records for cancellation analysis

Excluded them from trip duration and revenue calculations

Encoded categorical variables such as ride type, payment method, and weather

Categorized hours into peak and off-peak periods

Exploratory Data Analysis
Temporal Demand Patterns

Two major daily demand peaks observed:

Morning peak: 8–10 AM

Evening peak: 6–8 PM

Highest supply shortages occurred between 6–7 PM

Weekday evenings dominated by commute-related trips

Weekend mornings showed increased leisure travel demand

Cancellations and No Cars Available

Cancellation rates increase to approximately 25% during peak hours

“No Cars Available” events are concentrated in high-density pickup zones such as Majestic and Koramangala

Revenue and Ride-Type Analysis

UberGo accounts for approximately 33% of trips but contributes only 28% of total revenue

UberXL represents around 32% of trips while contributing nearly 40% of total revenue

Average tip amount shows a positive correlation with trip duration (correlation coefficient ≈ 0.45)

Data Visualization

Heatmaps showing request volume by hour and pickup zone

Line charts illustrating hourly request volume and fulfillment rate

Bar charts displaying cancellation and “No Cars Available” rates by ride type

Box plots comparing wait times and trip durations across ride types

Scatter plots of trip cost versus duration, segmented by weather conditions

Weather Impact & Trend Analysis

Rainy and stormy weather conditions result in:

Approximately 20% increase in “No Cars Available” events

Around 15% higher cancellation rates

Late-night demand shows month-over-month growth without a proportional increase in driver availability

Key Insights

Peak-hour supply shortages are the primary drivers of cancellations

Adverse weather significantly worsens ride fulfillment rates

UberXL is a high-value ride category with disproportionate revenue contribution

Recommendations

Implement dynamic driver incentive schemes during peak hours and adverse weather

Reallocate drivers in real time to high-demand pickup zones

Promote underutilized ride tiers through targeted marketing strategies

Deliverables

Fully documented and annotated Jupyter Notebook

Clear visualizations highlighting key patterns

Actionable insights and data-driven recommendations
