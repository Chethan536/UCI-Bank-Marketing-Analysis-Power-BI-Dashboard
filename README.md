# 📊 UCI Bank Marketing Data Analysis & Power BI Dashboard

This project analyzes the **UCI Bank Marketing Dataset** using **Python** for data cleaning and EDA, and **Power BI** for interactive visualizations. It uncovers customer behavior patterns, financial trends, call performance insights, and subscription drivers to help improve marketing strategy and business decision-making.

---

## 📌 Project Overview

The dataset includes customer demographics, financial details, and marketing campaign call records from a Portuguese bank.
The goal is to identify **which customers are most likely to subscribe** to a term deposit and **what factors influence campaign success**.

This project answers:

* How many married individuals are unemployed?
* How do job and marital status affect customer response?
* What is the average age of subscribers?
* How does customer balance vary across months?
* What is the average call duration per month?
* How does education relate to marital status?
* Which demographic groups convert the most?
* What is the impact of previous campaign outcome on subscription?

---

## 📘 Project Description

### 🐍 Python (Data Cleaning & EDA)

* Handled missing values and duplicates
* Standardized column names and data types
* Created derived fields (AgeGroup, MonthName, Duration Bins)
* Conducted EDA on demographics, balances, call durations, responses

### 📊 Power BI (Interactive Dashboard)

* 3-page interactive dashboard
* KPIs, trend charts, segmentation visuals, call-performance charts
* DAX measures, slicers, grouping/bins
* Clean storytelling layout focused on marketing analytics

---

## 🛠 Tools & Technologies

* **Python:** Pandas, NumPy, Matplotlib, Seaborn
* **Power BI:** Power Query, DAX, Slicers, Binning
* **Skills:** EDA, Data Cleaning, Segmentation, Marketing Analytics, Dashboard Design

---

## 📈 Power BI Dashboard Pages

### 📄 Page 1 — Executive Summary

**KPIs:**

* Total Contacts
* Total Subscriptions
* Conversion Rate
* Average Balance
* Average Call Duration

**Trends:**

* Subscriptions by Month
* Average Balance by Month
* Average Call Duration by Month

---

### 📄 Page 2 — Customer Segmentation

**Visuals:**

* Subscriptions by Job
* Subscriptions by Education
* Subscriptions by Marital Status
* Average Balance by Job

---

### 📄 Page 3 — Call Performance & Campaign Effectiveness

**Visuals:**

* Call Duration Distribution
* Subscription vs Non-Subscription
* Average Balance by Job
* Previous Campaign Outcome Impact

---

## 📊 DAX Measures Used

```dax
Total Contacts = COUNTROWS(bank)

Total Subscriptions =
CALCULATE(
    COUNTROWS(bank),
    bank[y] = "Yes"
)

Conversion Rate =
DIVIDE([Total Subscriptions], [Total Contacts], 0)

Avg Call Duration = AVERAGE(bank[duration])

Avg Balance = AVERAGE(bank[balance])
```

---

## 🔍 Key Insights

### 👤 Customer Insights

* Management & Technician roles convert the most
* Married customers subscribe more frequently
* Secondary education group shows highest conversions

### 💰 Financial Insights

* Retired customers have the highest average balance
* Balance trends vary month-to-month

### 📞 Call Behavior Insights

* Most calls are under 200 seconds
* Longer calls slightly increase subscription chance
* Overall conversion ≈ **12%**

### 🎯 Campaign Insights

* Best subscription months: **April–July**
* Positive previous outcomes strongly boost success rate

---

## 🎯 Why This Project Matters

This project demonstrates:

* End-to-end analytics workflow
* Strong Python EDA + Power BI dashboarding
* DAX measure creation & storytelling
* Customer segmentation & marketing analytics
* Ability to turn raw data → actionable insights

Great for **Data Analyst**, **BI Analyst**, and **Data Science** portfolios.

---

## 📂 Recommended Folder Structure

```
UCI-Bank-Project/
│
├── bank.csv
│   
├── Bank_project.ipynb
│
├── UCI_Bank_Marketing.pbix
│
├── dashboard_screenshots/
│
└── README.md
```

---






