# P15_Airline-Passenger-Satisfaction

**VERSION 1**

**A. Project Overview**

- This project analyzes airline passenger satisfaction by cleaning, visualizing and analyzing customer survey and flight delay data to uncover key service pain points & propose actionable improvements.

_Explore more insights in the full Power BI dashboard_

**B. Dataset Information**

**Source**

- Name: Airline Passenger Satisfaction
- From Kaggle

https://www.kaggle.com/datasets/teejmahal20/airline-passenger-satisfaction/data

**Notes**

- In this version, we just use train.csv file for EDA to find service improvement strategy, customer retention & define loyalty program
- However, when make data cleaning, I will do for both files: train & test in order to save time when doing version 2 - Predictive Analysis

**C. Methodology**

- I. Data Cleaning:
  + Column Types checked.
  + Missing values:
    - Train: Arrival Delay in Minutes has 310 blanks (~0.3%) → dropped.
    - Test: Arrival Delay in Minutes has 83 blanks (~0.3%) → dropped.
  + Zero values:
    - Train:
      + Departure Delay (56.52%), Arrival Delay (56.14%) → numeric metrics → must handle.
      + Other service scores (0.01–5%) → not critical, ignore.
    - Test: Similar pattern.
  → Handling: Fill delay minutes with median (from train), as delays are right-skewed (most flights delay few minutes, some >1000 minutes).
  + Outliers (IQR Rule):
    - Train: Departure Delay 42.7%, Arrival Delay 43.1%
    - Test: Departure Delay 42.7%, Arrival Delay 42.8%
  → Very high ratio; this reflects true distribution, not data error. Keep for Version 1 (BI).
  → Grouping: <15 mins, 15–60 mins, >60 mins.
- Export:
  + Version 1 (Insight): train_cleaned.csv
  + Version 2 (Predictive): Apply capping, then export train_cleaned_v2.csv & test_cleaned_v2.csv.
- Using Power BI for Dashboard visualize & find insights.

**D. Key Findings & Actionable Plans**

**_Key Findings_**

- Majority customers are 36–60 years old, followed by 18–35. Business & Eco classes dominate equally (~48% vs ~45%).
- ~57% customers are not satisfied or only neutral, mainly due to significant departure and arrival delays (~14% flights delayed over 1 hour).
- Overall customer evaluation is ~3/5 → moderate.
- Business class has the highest service ratings (3.6–3.8), especially inflight service and baggage handling. Weakest are food & drink (3.2) and inflight wifi (2.7) → directly impacting the largest segment, business travelers (47.8%).
- Fast & Convenience score lower (~3.0), with strengths in check-in and onboarding, but weaknesses in gate location (2.98) and online booking (2.76). → directly impacting the ecommerce online booking segment

**_Actionable Plans_**

- Short-term (Operational Fixes):
  + Improve Wifi speed (High): reassess infrastructure & contracts.
  + Fix online booking gaps (High): IT team audit booking flow, while maintaining strong onboarding process.
  + Reduce departure & arrival delays (High):
    - Allocate more staff during peak hours.
    - Improve Collaboration Quality with airports for better gate allocation → reduce waiting and circling.
  + Enhance Food & Drink quality (Medium): review current suppliers, renegotiate or change.
  + Promotions for leisure travelers (Low): stimulate non-business demand.
- Long-term (Strategic Initiatives):
  + Predictive delay model (High): use historical + weather + schedule data to forecast risk and mitigate proactively.
  + Improve ATC coordination (Medium): implement real-time communication to adjust routes dynamically.
  + Expand gate capacity (Medium): optimize gate layout to ease passenger movement.

_**About Me**_

Hi, I'm Navin (Bao Vy) – an aspiring Data Analyst passionate about turning raw data into actionable business insights.
I’m eager to contribute to data-driven decision making and help organizations translate analytics into business impact.
For more details, please reach out at:

🌐 LinkedIn: https://www.linkedin.com/in/navin826/

📂 Portfolio: https://github.com/CallmeNavin/
