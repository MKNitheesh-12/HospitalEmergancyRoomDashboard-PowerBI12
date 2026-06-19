# Hospital ER Patient Analytics Dashboard 🏥

A Power BI dashboard (`my_pbi34.pbix`) that analyzes hospital Emergency Room (ER) patient data — admissions, wait times, demographics, and satisfaction scores — across three interactive report pages.

## 📊 Overview

This report connects to a single fact table (`Hospital ER_Data`) plus a `Date Table` for time intelligence, and visualizes key ER operational metrics such as patient volume, wait times, admission status, and patient satisfaction.

## 📁 Report Pages

### 1. Monthly View
A month-by-month breakdown of ER activity, including:
- Area charts trending patient volume, wait time, and related KPIs over time
- KPI cards for quick-glance metrics
- **Patient Admission Status** (pivot table)
- **% of Patients Seen Within 30 Min** (donut chart)
- **No of Patients by Gender** (donut chart)
- **No of Patients by Day and Hour** (column chart)
- Bar/column charts for additional breakdowns
- Slicers for filtering by date/period

### 2. Consolidated View
A summary page mirroring the Monthly View's visuals but aggregated across the full dataset (no monthly split) — useful for a high-level, all-time snapshot of:
- Patient Admission Status
- % of Patients Seen Within 30 Min
- No of Patients by Gender
- No of Patients by Day and Hour

### 3. Patients Details
A detail-level page featuring a searchable/filterable data table of individual patient records, with slicers to drill into specific patients.

## 🗂️ Data Model

| Table | Purpose |
|---|---|
| `Hospital ER_Data` | Main fact table containing patient-level ER records |
| `Date Table` | Supporting date dimension for time-based filtering and trending |

### Key Fields

| Field | Description |
|---|---|
| Patient Id | Unique patient identifier |
| Patient Full Name | Patient name |
| Patient Age / Age Group | Patient age and age bucket |
| Patient Gender | Patient gender |
| Patient Race | Patient race/ethnicity |
| Admission Status / Patient Admission Flag | Whether the patient was admitted |
| Department Referral | Department the patient was referred to |
| No of Patients | Patient count measure |
| No of Patient Referred | Referral count measure |
| Patient Waittime / Avg Wait Time | Time patient waited to be seen |
| Waittime Interval / Waittime Status | Bucketed wait-time category |
| Satisfication Score | Patient satisfaction rating |
| Date / Month Name / Month & Year / Day Name / Year | Date dimension attributes |

## 🛠️ Tech Stack
- **Power BI Desktop** (.pbix)
- DAX measures for KPIs (patient counts, average wait time, etc.)
- Visuals: area charts, column/bar charts, donut charts, pivot tables, cards, slicers

## 🚀 Getting Started

1. Clone or download this repository.
2. Open `my_pbi34.pbix` in [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free).
3. If prompted, point the data source connection to your own copy of the ER dataset, or use the embedded data as-is.
4. Use the slicers on each page to filter by date, department, gender, or admission status.
5. Navigate between pages using the in-report page navigator buttons.

## 📌 Notes
- Replace this section with any data-source/privacy notes relevant to your actual patient data (e.g., anonymization, sample/demo data disclaimer) before publishing if the dataset contains real patient information.
- Consider adding a screenshot/GIF of each report page here for visual context (GitHub renders images well in READMEs).

---
*Feel free to adjust wording, badges, or add a license section depending on how you intend to share this repo.*
