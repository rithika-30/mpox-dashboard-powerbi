🌍 Mpox (Monkeypox) Global Outbreak Dashboard

**Overview**

This project presents an interactive dashboard created using **Power BI** that tracks the **Mpox (Monkeypox) global outbreak** between **2022 and 2023**, based on real data from (https://www.kaggle.com/datasets/utkarshx27/mpox-monkeypox-data/data). The dashboard offers insights into:
- Cumulative case trends across countries
- Geographic spread of cases
- Mortality rate analysis
- Country-wise comparisons


## 📊 Dataset

- **Source:** https://www.kaggle.com/datasets/utkarshx27/mpox-monkeypox-data/data
- **File Used:** `owid-monkeypox-data.csv`
- **Key Fields:**
  - `date` – Reporting date
  - `location` – Country/region
  - `total_cases`, `new_cases`
  - `total_deaths`, `new_deaths`

---

## 🛠️ Tools & Technologies

- **Power BI** – For dashboard creation
- **Power Query Editor** – For data cleaning and shaping
- **DAX (Data Analysis Expressions)** – For calculating mortality rate and custom measures

---

## 📈 Key Visualizations

- 📉 **Line Chart:** Cumulative total cases over time per country
- 🌐 **Map Visualization:** Total cases by country
- 🧾 **KPI Cards:** Total confirmed cases, total deaths, and mortality rate
- 🎛️ **Slicers:** Filter by country and date

---

## 🧠 Key Insights

- **Brazil** and **the United States** showed the highest number of confirmed cases.
- The **mortality rate** globally remained low, below 0.1%.
- Most outbreaks occurred between **June 2022 and March 2023**.
- **Geographical spread** revealed Mpox cases in over 100 countries.

---

## 💡 DAX Measures Used

```DAX
Mortality Rate = DIVIDE(SUM('Table'[total_deaths]), SUM('Table'[total_cases]))
