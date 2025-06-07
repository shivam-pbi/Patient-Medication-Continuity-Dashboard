# 💊 Patient Medication Continuity Dashboard – Power BI / SQL / Excel

This dashboard visualizes MRN (Medical Record Number) activity trends across time and geography, helping healthcare teams understand patient medication continuity and identify high-risk drop-off zones.

![Sample_5_page-0001](https://github.com/user-attachments/assets/9dbff27d-5c70-4f7d-98ef-f7c2a929ba33)

---

## 🔍 Purpose

The objective of this dashboard was to:
- Track patient medication adherence and identify inactivity/discontinuity trends
- Compare city-wise and zip-code-level MRN activity for targeted healthcare interventions
- Enable quick cohort analysis to monitor medication engagement over months

This tool was primarily intended for **healthcare analytics teams**, **clinical operations managers**, and **public health strategists**.

---

## 🎯 Business Impact

- 📉 **Identified early medication drop-off patterns**, helping in proactive patient follow-ups
- 📍 **Mapped MRN distribution** across cities and zip codes to detect underserved or at-risk zones
- 🔁 **Cohort retention charts** enabled month-on-month tracking of patient engagement
- 💡 Informed targeted **outreach campaigns in regions with <30% active MRNs**

---

## 🛠️ How It Was Built

**Data Assumptions:**
- Blank access dates assumed as `30-Dec-1899` to flag discontinuity
- Patients assumed to have a 10-month prescription window (`Month_0` to `Month_9`)
- All MRNs were evaluated based on their most recent activity to classify status

**Power BI Features Used:**
- DAX-based logic to derive **active vs inactive MRN counts**
- Conditional formatting to flag first inactive month
- Map visuals for **MRN density by area and zip code**
- Cohort analysis matrix to track engagement drops over time
- City comparison charts with calculated **discontinuity rates**

---

## 🖼️ Key Visuals

- 🔹 **MRN Activity Over Time** – Active vs Inactive across 10 months
- 🔹 **Top & Bottom Performing Cities** – Discontinuity comparison (Austin vs Dallas)
- 🔹 **MRN Density by Zip Code** – Geographic hotspots
- 🔹 **Cohort Retention Matrix** – Engagement percentage by start month
- 🔹 **Focus Areas for Improvement** – Cities with lowest active MRNs

---

## 📌 Key Takeaways

- 📉 **Only ~38% of MRNs remain active** after 10 months from medication initiation
- 🏙️ **Dallas showed a higher discontinuity rate (64%) compared to Austin (55%)**
- 📍 **Zip codes like 78741, 78744 (Austin) and 75206 (Dallas)** showed relatively higher active MRNs
- 🚨 **Houston, Garland, Richardson, and Georgetown** were identified as bottom 5 areas needing intervention

---

## 🧰 Tools Used

- Power BI Desktop
- SQL Server
- Excel-based data export
- DAX & Power Query for MRN classification and time-based logic
