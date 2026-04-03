# 📦 Logistics Analytics Dashboard

> **An end-to-end Excel analytics project** — from raw shipment data to an interactive, dark-themed dashboard with slicers, pivot tables, and KPI cards.

![Dashboard Preview](Logistics_Analytics_Dashboard.png)

---

## 🚀 Project Overview

This project transforms a real-world logistics dataset of **2,000 shipments** into a fully interactive Excel dashboard. It showcases the complete analytics workflow: data cleaning, pivot table modeling, KPI engineering, and professional dashboard design — all without a single line of code.

The dashboard enables analysts to filter by **carrier**, **date range**, and **destination** to instantly surface performance insights across cost, delivery rate, transit time, and shipment volume.

---

## ✨ Features

| Feature | Description |
|---|---|
| 🎛️ **Interactive Slicers** | Filter by carrier (Amazon, DHL, FedEx, LaserShip, OnTrac, UPS, USPS) and date |
| 📊 **KPI Cards** | Total Shipments · Delivery Rate · Avg Cost · Avg Transit Days · Avg Miles |
| 🍩 **Gauge Chart** | Circular delivery rate indicator for the selected carrier |
| 📅 **Monthly Trend Line** | Shipment & delivery count across all 12 months |
| 🏙️ **Top 7 Destinations** | Ranked by delivery rate with horizontal bar chart |
| 💰 **Carrier Avg Cost** | Side-by-side cost comparison across all carriers |
| ⚖️ **Carrier Avg Weight** | Average package weight per carrier |
| ⏱️ **Carrier Avg Delivery Days** | Average transit time per carrier |

---

## 🗂️ Project Structure

```
logistics-dashboard/
│
├── 📊 Logistics_Analytics_Dashboard.xlsx   # Main Excel workbook
│   ├── Sheet: Database                      # Raw dataset (2,000 rows)
│   ├── Sheet: Analytics (Pivot Tables)      # All pivot table calculations
│   └── Sheet: Dashboard                     # Final interactive dashboard
│
├── 📁 logistics_dataset.csv                 # Source data file
│
└── 📸 screenshots/
    ├── Logistics_Analytics_Dashboard.png    # Full dashboard view
    ├── Logistics_Analytics_KPIs.png         # KPI section close-up
    ├── Showcasing_Pivot_Table.png           # Pivot table structure
    └── Used_pptx_to_create_a_base_for_dashboard.png  # Layout planning stage
```

---

## 🗃️ Dataset

**File:** `logistics_dataset.csv`  
**Records:** 2,000 shipments | **Year:** 2023

| Column | Description |
|---|---|
| `Shipment_ID` | Unique identifier (e.g. SH10000) |
| `Origin_Warehouse` | Dispatch location |
| `Destination` | Delivery city |
| `Carrier` | Shipping provider |
| `Shipment_Date` | Date parcel was sent |
| `Delivery_Date` | Date parcel was delivered |
| `Weight_kg` | Package weight |
| `Cost` | Shipment cost in USD |
| `Status` | Delivered / In Transit / etc. |
| `Distance_miles` | Route distance |
| `Transit_Days` | Days in transit |

**Carriers covered:** Amazon · DHL · FedEx · LaserShip · OnTrac · UPS · USPS

---

## 📐 How It Was Built

### Step 1 — Layout Planning in PowerPoint
The dashboard wireframe was designed in PowerPoint first, using dark-themed rounded rectangles to plan the card layout before building it in Excel. This ensured the visual hierarchy was intentional before any data was connected.

![PowerPoint Layout Base](Used_pptx_to_create_a_base_for_dashboard.png)

### Step 2 — Data Modeling with Pivot Tables
All metrics are powered by pivot tables with custom calculated fields. A dedicated `KPI measures` group handles dynamic calculations for Delivery Rate, AVG Cost, AVG Transit Days, and more — all updating in real time when slicers are applied.

![Pivot Tables](Showcasing_Pivot_Table.png)

### Step 3 — KPI Engineering
Six headline KPIs were engineered from the raw data and displayed as formatted cards at the top of the dashboard.

![KPIs](Logistics_Analytics_KPIs.png)

### Step 4 — Dashboard Assembly
Charts were built directly from pivot tables and embedded in the dashboard sheet. The PowerPoint wireframe was used as a background layout guide, then replaced with live Excel shapes, charts, and slicers.

---

## 📈 Key Insights

- 🏆 **Atlanta** leads all destinations with an **89% delivery rate**
- 💸 **USPS** offers the lowest average cost at **$183.18** per shipment
- ⚡ **FedEx** packages are the heaviest on average at **46.27 kg**
- 📅 **August** saw the highest shipment volume of the year (**182 shipments**)
- 🚚 **UPS** achieves the highest carrier delivery rate at **86%**
- ⏱️ **USPS & LaserShip** are the fastest carriers at an average of **4.0 transit days**

---

## 🛠️ Tools Used

![Excel](https://img.shields.io/badge/Microsoft_Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)
![PowerPoint](https://img.shields.io/badge/Microsoft_PowerPoint-B7472A?style=for-the-badge&logo=microsoft-powerpoint&logoColor=white)

- **Microsoft Excel** — Pivot Tables, Calculated Fields, Slicers, Charts, Conditional Formatting
- **Microsoft PowerPoint** — Dashboard wireframing and layout planning
- **CSV / Raw Data** — Data cleaning and preparation

---

## 💡 Skills Demonstrated

- ✅ Data cleaning and transformation in Excel
- ✅ Pivot table design with custom KPI measures
- ✅ Dynamic dashboard creation with slicers and timelines
- ✅ Data visualization (bar charts, line charts, gauge/donut charts)
- ✅ Dashboard UI/UX design — dark theme, consistent color language
- ✅ Iterative layout planning (PowerPoint → Excel workflow)

---

## 🖥️ Getting Started

1. **Clone or download** this repository
2. Open `Logistics_Analytics_Dashboard.xlsx` in **Microsoft Excel** (2016 or later recommended)
3. Navigate to the **Dashboard** sheet
4. Use the **carrier buttons** at the top or the **date slicer** on the right to filter the data
5. All charts and KPIs update automatically

> ⚠️ Some features (slicers, pivot charts) may not render correctly in Google Sheets or LibreOffice. Excel desktop is recommended.

---

## 📬 Contact

Have questions or feedback? Feel free to open an issue or reach out!

---

*Built with 📊 Excel and a lot of attention to detail.*
