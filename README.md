# Smart City Citizen Complaint Dashboard — Power BI Capstone Project

An interactive Power BI dashboard built on a Smart City dataset to analyze citizen complaints, resolution efficiency, department performance, and AI-driven priority scoring across city sectors.

---

## Project Overview

Urban municipalities receive thousands of citizen complaints daily — garbage, traffic, water issues, potholes, and more. This project builds a comprehensive Power BI dashboard to help city administrators:

- Monitor complaint volume and severity across sectors
- Track resolution time and department performance
- Identify high-priority areas using AI Priority Score
- Understand citizen satisfaction trends

---

## Dataset

**File:** `SmartCity_Cleaned.csv`  
**Records:** 1,006 rows | **Columns:** 13

| Column | Description |
|---|---|
| `Citizen_ID` | Unique citizen identifier |
| `Area_Sector` | City sector (A1, A2, B1, B2, C1, C2, D1, D2) |
| `Issue_Type` | Type of complaint |
| `Complaint_Text` | Description of the issue |
| `Severity_Level` | Critical / High / Medium / Low |
| `Reported_Time` | Timestamp when complaint was filed |
| `Resolution_Time_Hours` | Hours taken to resolve the complaint |
| `Assigned_Department` | Department handling the complaint |
| `Satisfaction_Rating` | Citizen satisfaction score (1–10) |
| `Followup_Required` | Whether a follow-up is needed (Yes/No) |
| `Latitude` | Geographic latitude |
| `Longitude` | Geographic longitude |
| `AI_Priority_Score` | AI-generated priority score (0.0–1.0) |

---

## Issue Types Covered

`Garbage` · `WiFi Issue` · `Traffic` · `Pothole` · `Water` · `Street Light` · `Pollution`

## Departments

`Cleanliness Dept` · `Electricity Dept` · `Smart WiFi Dept` · `Water Dept` · `Roads Dept`

---

## Dashboard Highlights

### 1. Complaint Overview
- Total complaints by Issue Type and Severity Level
- Sector-wise complaint distribution (A1–D2)
- Critical vs. High vs. Medium vs. Low breakdown

### 2. Resolution Performance
- Average resolution time by department
- Resolution Time distribution (Avg: ~82 hrs, Max: 999 hrs)
- Complaints requiring follow-up (Yes/No split)

### 3. Citizen Satisfaction
- Average satisfaction rating by issue type and sector
- Correlation between resolution time and satisfaction
- Low-satisfaction hotspots across the city

### 4. AI Priority Analysis
- AI Priority Score distribution (0.0–1.0)
- High-priority complaints mapped by sector and issue type
- Departments with highest pending critical issues

### 5. Geo Map View
- Complaint locations plotted using Latitude & Longitude
- Sector-level heatmap of complaint density

---

## Key Insights

- Complaints are spread across **8 city sectors** (A1–D2)
- Average resolution time is **~82 hours**, with outliers going up to **999 hours**
- Average citizen satisfaction is **3.15 / 10** — indicating significant room for improvement
- AI Priority Score averages **0.52**, helping departments triage critical cases faster
- A notable portion of complaints require **follow-up**, highlighting unresolved issues

---

## Tools Used

- **Power BI Desktop** — Dashboard creation and visualization
- **Python / Excel** — Data cleaning and preprocessing
- **Dataset:** SmartCity_Cleaned.csv

---

## Project Structure

```
smartcity-dashboard/
│
├── Capstone_project.pbix       # Power BI dashboard file
├── SmartCity_Cleaned.csv       # Cleaned dataset
└── README.md
```

---

## How to Use

1. Download and install [Power BI Desktop](https://powerbi.microsoft.com/desktop/)
2. Clone or download this repository
3. Open `Capstone_project.pbix` in Power BI Desktop
4. Ensure `SmartCity_Cleaned.csv` is in the same folder (or update the data source path)
5. Refresh the data and explore the dashboard

