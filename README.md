# 🏥 Hospital Emergency Room Dashboard

## 📌 Project Overview
This project presents an end-to-end **Hospital Emergency Room Analytics Dashboard** designed to analyze patient flow, wait times, admissions, and department referrals.  
The goal is to help healthcare stakeholders improve operational efficiency and patient experience.

---

## 🎯 Objectives
- Monitor ER patient volume and trends
- Analyze average wait time and delays
- Understand admission vs non-admission rates
- Identify peak days and operational bottlenecks
- Track department referrals and age distribution

---

## 📊 Key Metrics (KPIs)
- Total Number of Patients  
- Average Wait Time (Minutes)  
- Patient Satisfaction Score  
- Admission Status  
- Timeliness (On-Time vs Delayed)  
- Gender-wise & Age-group Analysis  

---

## 📈 Visual Insights
- Monthly ER performance overview
- Daily patient arrival trends using area charts
- Wait time trends to identify improvement areas
- Department-wise referral analysis

---

## 🛠 Tools & Technologies
- Power BI  
- Microsoft Excel  
- DAX (Calculated Columns & Measures)  
- Data Modeling & Visualization  

---

## 📂 Dataset
The dataset contains anonymized emergency room patient records including:
- Patient Age & Gender  
- Wait Time  
- Admission Status  
- Department Referrals  
- Visit Date  

---

## 🧮 DAX Highlights
```DAX
Age Group = 
IF([Patient Age]>=70,"70-79",
IF([Patient Age]>=60,"60-69",
IF([Patient Age]>=45,"45-59",
IF([Patient Age]>=30,"30-44",
IF([Patient Age]>=15,"15-29",
IF([Patient Age]>=5,"05-14","0-4"))))))
