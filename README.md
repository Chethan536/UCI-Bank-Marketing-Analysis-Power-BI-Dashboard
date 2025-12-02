# UCI-Bank-Marketing-Analysis-Power-BI-Dashboard

````md
# 📊 UCI Bank Marketing Data Analysis & Power BI Dashboard

An end-to-end analytics project exploring the **UCI Bank Marketing Dataset** using  
**Python (Pandas, NumPy, Seaborn, Matplotlib)** and **Power BI** to uncover customer behavior, financial patterns, and marketing campaign effectiveness.

This project demonstrates complete data processing → EDA → insights → dashboard storytelling.

---

## 🧭 Table of Contents
- [📌 Project Overview](#-project-overview)
- [📘 Project Description](#-project-description)
- [🛠 Tools & Technologies](#-tools--technologies)
- [📈 Dashboard Pages](#-dashboard-pages)
  - [Page 1: Executive Summary](#page-1-executive-summary)
  - [Page 2: Customer Segmentation](#page-2-customer-segmentation)
  - [Page 3: Call Performance Insights](#page-3-call-performance-insights)
- [📊 DAX Measures](#-dax-measures)
- [🔍 Key Insights](#-key-insights)
- [🎯 Why This Project Matters](#-why-this-project-matters)
- [📂 Folder Structure](#-folder-structure)
- [🤝 Contributing](#-contributing)

---

# 📌 Project Overview
This project analyzes the **UCI Bank Marketing Dataset** to understand:

- Customer behavior  
- Demographic trends  
- Subscription patterns  
- Call performance  
- Financial insights  
- Marketing campaign effectiveness  

Using Python for data cleaning & exploration and Power BI for interactive dashboards, the project reveals patterns that help improve targeting, optimize call strategies, and enhance decision-making.

---

# 📘 Project Description
The goal of this project is to explore how customer demographics, employment status, financial health, and call behaviors influence term deposit subscription rates.

Using Python, we cleaned, transformed, and analyzed the dataset to answer key business questions:

### ✔ Key Questions Answered
- How many married individuals are unemployed?  
- What is the average age of customers who subscribed?  
- How do customer balances vary month to month?  
- Which job roles convert the most?  
- How does call duration impact subscription?  
- What is the subscription distribution across education levels?  
- How does previous campaign outcome affect conversion?  

These insights form the basis for optimized marketing campaigns and customer segmentation.

---

# 🛠 Tools & Technologies

### **Python (EDA & Cleaning)**
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  

### **Power BI (Dashboard)**
- DAX Measures  
- Slicers & filters  
- Binning & grouping  
- Multi-page analysis  
- Trend, bar, column, and distribution visuals  

---

# 📈 Dashboard Pages

## **📄 Page 1: Executive Summary**
High-level campaign performance overview.

### ⭐ KPIs
- Total Contacts  
- Total Subscriptions  
- Conversion Rate  
- Avg Balance  
- Avg Call Duration  

### 📊 Trend Visuals
- Subscriptions by Month  
- Avg Balance by Month  
- Avg Call Duration by Month  

### 🎛 Filters
- Month  
- Job  
- AgeGroup  

---

## **📄 Page 2: Customer Segmentation**
Detailed look at customer demographics.

### 📊 Visuals
- Subscriptions by Job  
- Subscriptions by Education  
- Subscriptions by Marital Status  
- Avg Balance by Job  

### 🎛 Filters
- Education  
- Job  
- Marital  
- AgeGroup  

---

## **📄 Page 3: Call Performance Insights**
Call behavior and campaign effectiveness.

### 📊 Visuals
- Call Duration Distribution (Histogram)  
- Subscription vs Non-subscription  
- Avg Balance by Job  
- Impact of Previous Campaign Outcome  

### 🎛 Filters
- Previous Outcome  
- AgeGroup  
- Month  
- Job  

---

# 📊 DAX Measures

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
````

---

# 🔍 Key Insights

### 👤 Customer Insights

* Management & Technician roles show highest engagement.
* Married customers subscribe more often.
* Secondary education group has highest conversions.

### 💰 Balance & Financial Insights

* Retired customers hold the highest balances.
* Customer balance varies seasonally across months.

### 📞 Call Behavior Insights

* Most calls are short (under 200 seconds).
* Longer calls slightly increase subscription chances.
* Subscription rate is ~12% (521 out of 4521 contacts).

### 🎯 Campaign Strategy Insights

* Subscription peaks between **April–July**.
* Positive previous outcome increases conversion likelihood.

---

# 🎯 Why This Project Matters

This project demonstrates:

* End-to-end data analysis workflow
* Data cleaning, transformation & segmentation
* Business storytelling with Power BI
* Real-world marketing & customer behavior insights
* Strong analytical and visualization skills

Great for Data Analyst, BI Analyst, and Data Science roles.

---

# 📂 Folder Structure

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

# 🤝 Contributing

Feel free to fork the repo, raise issues, or suggest improvements.
Feedback is always welcome!

---

# ⭐ If you found this project useful…

Consider giving the repository a **star** 🌟 on GitHub!


