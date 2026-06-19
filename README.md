# 🏥 Hospital Emergency Room (ER) Dashboard — Power BI

An interactive Power BI dashboard that analyzes Hospital Emergency Room (ER) operations, giving hospital management visibility into patient volume, wait times, satisfaction, demographics, and department referrals to support faster, data-driven operational decisions.

## 📌 Overview

This dashboard is built on a single fact table (`Hospital ER_Data`) joined to a `Date Table`, and is organized into three report pages: a monthly trends view, a consolidated/summary view with a flexible date range, and a patient-level detail table.

## 📊 Key Metrics

| Metric | Value |
|---|---|
| Total Patients Analyzed | 9,216 |
| Average Wait Time | 35.3 minutes |
| Patient Satisfaction Score | 4.99 / 5 |
| Patients Referred to Departments | 3,816 |

## 🗂️ Report Pages

### 1️⃣ Monthly View
- Trends in patient volume, admission status, and referrals
- Patient demographics: age, race, gender
- Patient volume by day and hour
- Admission status breakdown (pivot table)
- % of patients seen within 30 minutes (donut chart)
- Patient distribution by gender (donut chart)

### 2️⃣ Consolidated View
- Summary KPIs over a customizable date range (slicer-driven)
- Same suite of trend and operational visuals as the Monthly View, rolled up for flexible period-over-period analysis

### 3️⃣ Patients Details
- Granular, patient-level data table for drill-through and ad hoc analysis
- Fields: Patient ID, Patient Full Name, Gender, Age, Wait Time, Admission Status, Department Referral

## 🔍 Visuals Used

- **Area charts** — daily trend sparklines for patient volume, average wait time, satisfaction score, and department referrals
- **Donut charts** — % of patients seen within 30 minutes; patient distribution by gender
- **Clustered bar / column charts & column chart** — demographic breakdowns and patients by day and hour
- **Pivot tables** — patient admission status and other cross-tab summaries
- **Cards** — headline KPIs (total patients, avg. wait time, satisfaction score, referrals)
- **Slicers** — date range and other filters
- **Table** — patient-level detail grid

## 🧱 Data Model

| Table | Description |
|---|---|
| `Hospital ER_Data` | Core fact table: Patient Id, Patient Full Name, Patient Gender, Patient Age, Age Group, Patient Race, Patient Waittime, Avg Wait Time, Waittime Interval, Waittime status, Satisfication Score, Admission Status, Patient Admission Flag, Department Referral, No of Patients, No of patient Referred |
| `Date Table` | Date dimension: Date, Day Name, Month Name, Year (used for time intelligence and the Date Hierarchy) |

## 🛠️ Tools Used

- **Power BI Desktop** — data modeling, DAX measures, and report design

## 🚀 How to Use

1. Clone or download this repository.
2. Open `my_pbi34.pbix` in **Power BI Desktop**.
3. Use the date slicers on the Monthly View / Consolidated View pages to filter the period of analysis.
4. Navigate between pages using the in-report page navigator buttons.
5. Drill into individual patients on the **Patients Details** page.

## 📁 Repository Structure

```
├── my_pbi34.pbix     # Power BI report file
└── README.md         # Project documentation
```

## 💡 Key Takeaway

This project demonstrates how Power BI can turn raw ER operational data into actionable insights — helping hospital management track patient flow, reduce wait times, and improve patient satisfaction through informed, data-backed decisions.
