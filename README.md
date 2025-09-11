# P15_Airline-Passenger-Satisfaction

**VERSION 1**

**A. Project Overview**

- This project 

_Explore more insights in the full Power BI dashboard_

**B. Dataset Information**

**Source**

- Name: Airline Passenger Satisfaction
- From Kaggle

https://www.kaggle.com/datasets/teejmahal20/airline-passenger-satisfaction/data

- In this version, we just use train.csv file for EDA - customer analysis by age, gender, class, loyalty, delay, service… to find service improvement strategy, customer retention & define loyalty program
- However, when make data cleaning, I will do for both files: train & test in order to save time when doing version 2 - Predictive Analysis

**C. Methodology**

- I. Data Cleaning:
  + Columns Types
  + %Blank/null:
    - train: Arrival Delay in Minutes blank column 310 value --> không đáng kể --> drop
    - test: Arrival Delay in Minutes column blank 83 --> không đáng kể --> drop
  + %Zero Value:
    - train:
      + Departure Delay in Minutes: 56.52 --> Nhóm numeric dạng đo lường --> Must handle
      + Arrival Delay in Minutes: 56.14 --> Nhóm numeric dạng đo lường --> Must handle
      + Departure/Arrival time convenient: 5.11 --> Score group --> Ignore
      + Ease of Online booking: 4.32 --> Score group --> Ignore
      + Inflight wifi service: 2.99 --> Score group --> Ignore
      + Online boarding: 2.34 --> Score group --> Ignore
      + Leg room service: 0.45 --> Score group --> Ignore
      + Food and drink: 0.10 --> Score group --> Ignore
      + Cleanliness: 0.01 --> Score group --> Ignore
      + Inflight entertainment: 0.01 --> Score group --> Ignore
    - test:
      + Departure Delay in Minutes: 56.61 --> Nhóm numeric dạng đo lường --> Must handle
      + Arrival Delay in Minutes: 56.36 --> Nhóm numeric dạng đo lường --> Must handle
      + Departure/Arrival time convenient: 5.31 --> Score group --> Ignore
      + Ease of Online booking: 4.61 --> Score group --> Ignore
      + Inflight wifi service: 3.14 --> Score group --> Ignore
      + Online boarding: 2.51 --> Score group --> Ignore
      + Leg room service: 0.49 --> Score group --> Ignore
      + Food and drink: 0.10 --> Score group --> Ignore
      + Inflight entertainment: 0.02 --> Score group --> Ignore
      + Cleanliness: 0.01 --> Score group --> Ignore
      + On-board service: 0.01 --> Score group --> Ignore
      + Inflight service: 0.01 --> Score group --> Ignore
   - Handle:
     + Fill by median (from train data to fill both file) because Delay minutes thường có phân phối lệch (Phần lớn chuyến delay ít phút hoặc không delay. Một số chuyến delay cực kỳ dài (1000 phút chẳng hạn).
  + Outliers: chỉ check 2 column - Departure Delay in Minutes, Arrival Delay in Minutes
    - train:
      + Departure Delay in Minutes
      + Arrival Delay in Minutes
    - test:
      + Departure Delay in Minutes
      + Arrival Delay in Minutes

**D. Key Findings & Actionable Plans**

**_Key Findings_**

- 

**_Actionable Plans_**

- 

_**About Me**_

Hi, I'm Navin (Bao Vy) – an aspiring Data Analyst passionate about turning raw data into actionable business insights.
I’m eager to contribute to data-driven decision making and help organizations translate analytics into business impact.
For more details, please reach out at:

🌐 LinkedIn: https://www.linkedin.com/in/navin826/

📂 Portfolio: https://github.com/CallmeNavin/
