# Bellabeat Case Study (Google Data Analytics Capstone)

**Author:** Catrina Moore  
**Date:** February 2026  
**Tools Used:** R, tidyverse, ggplot2, janitor, lubridate  

---

## Overview
Bellabeat is a high-tech company that manufactures health-focused smart products designed to inform and inspire women around the world. Bellabeat devices collect data on activity, sleep, stress, and reproductive health to empower users with insights about their health and habits.

This project analyzes **Fitbit Fitness Tracker Data** to understand how consumers use smart devices and to generate actionable marketing recommendations for the **Bellabeat Leaf wellness tracker**.

---

## Business Task
Analyze smart device usage data to gain insight into how consumers use non-Bellabeat smart devices. Apply these insights to one Bellabeat product and provide data-driven marketing recommendations to unlock new growth opportunities.

---

## Key Stakeholders
- **Urška Sršen** — Cofounder and Chief Creative Officer  
- **Sando Mur** — Mathematician and Cofounder (Bellabeat Executive Team)  
- **Bellabeat Marketing Analytics Team**

---

## Dataset
**FitBit Fitness Tracker Data (CC0: Public Domain)**  
Source: Kaggle (Mobius)  
Time period: 31 days (2016)  
Sample size: 33 users  

Files used in this analysis:
- `dailyActivity_merged.csv`  
- `sleepDay_merged.csv`  
- `hourlySteps_merged.csv`

---

## Data Credibility (ROCCC Assessment)
This dataset contains real Fitbit user data, but it has several limitations:

- **Reliability:** Real user activity and sleep logs, but sourced through a third party  
- **Originality:** Not collected directly by Bellabeat  
- **Comprehensiveness:** Limited to 33 users over 1 month  
- **Current:** Data is from 2016 (not current)  
- **Cited:** Public domain dataset hosted on Kaggle  

Additional limitations:
- No gender labels (Bellabeat primarily targets women)
- Short time window limits seasonal behavior insights

---

## Process Summary
This project followed the Google Data Analytics framework:

### 1. Ask
Defined the business task and identified key stakeholders.

### 2. Prepare
Selected and documented datasets and assessed credibility using ROCCC.

### 3. Process
Cleaned and formatted data in R:
- Renamed tables for consistency  
- Cleaned column names using `janitor::clean_names()`  
- Converted date columns to proper formats  
- Verified unique users and checked for duplicates  
- Removed duplicates from sleep data  
- Joined daily activity and sleep datasets into a combined table (`activity_sleep`)

### 4. Analyze
Performed exploratory analysis and created visualizations to identify trends in:
- Daily steps  
- Sedentary minutes  
- Sleep duration and time in bed  
- Activity level segmentation  

### 5. Share
Summarized key insights with supporting visuals.

### 6. Act
Delivered recommendations for marketing strategy and product positioning.

---

## Key Findings
- **High sedentary time exists even among active users**  
  Many users show long sedentary periods despite meeting step goals.

- **Users with more daily steps tend to sleep longer**  
  Increased activity is associated with longer sleep duration.

- **Most users fall into moderate activity categories**  
  A large portion of users are lightly or fairly active.

- **Step tracking appears stronger than sleep consistency tracking**  
  Sleep data coverage was lower than activity data, suggesting inconsistent tracking.

---

## Visualizations Included
This project includes key charts such as:
- Daily Steps vs Sedentary Minutes  
- Distribution of User Activity Levels  
- Minutes Asleep vs Time in Bed  
- Daily Steps vs Total Minutes Asleep  

(Charts can be found in the `outputs/figures/` folder if exported.)

---

## Recommendations (Bellabeat Leaf Tracker)
Based on the insights, the following marketing recommendations were developed:

### 1. Sedentary Behavior Campaign
Position the Leaf as a daily movement companion that supports:
- Push notifications to stand/move  
- Customizable reminders  
- Guided movement breaks  
- Lifestyle-based nudges for healthier habits  

### 2. Sleep Health Campaign
Emphasize sleep consistency and improve sleep features by:
- Helping users identify patterns affecting sleep (stress, caffeine, routines)  
- Supporting bedtime/wind-down routines  
- Offering gentle “optimal wake-up” features using motion detection  

### 3. Lifestyle-Based Personalization
Segment users into activity categories and personalize:
- Workout recommendations  
- Push notifications  
- Motivation messaging  
- Weekly goals  

Segments:
- Sedentary  
- Lightly Active  
- Fairly Active  
- Very Active  

---

## Conclusion
In this case study, I analyzed smart device usage data using R to identify trends in activity, sedentary behavior, and sleep. I cleaned, joined, and visualized multiple datasets to uncover actionable insights. Based on these findings, I developed marketing recommendations for Bellabeat’s Leaf wellness tracker focused on behavior nudges, sleep health, and personalized engagement.

---
