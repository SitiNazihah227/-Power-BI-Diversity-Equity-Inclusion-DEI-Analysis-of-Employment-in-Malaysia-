# Diversity, Equity & Inclusion (DEI) Analysis of Employment in Malaysia

A Power BI dashboard exploring workforce participation, salary distribution, and employment composition in Malaysia through the lens of gender, age group, ethnicity, and educational attainment.

---

## Overview

This dashboard provides a data-driven view of labour market equity in Malaysia. It is structured across two report pages, covering key DEI dimensions using publicly available official and community-sourced datasets.

| Page | Focus Area | Period Covered |
|------|-----------|---------------|
| Page 1 — Gender & Age Group | Labour force participation rates, salary gaps, industry breakdown | Q2 2022 – Q1 2025 *only salary gaps has no period range |
| Page 2 — Ethnic & Education Level | Ethnic group participation, education-level attainment and earnings | Q2 2022 – Q1 2025 |

---

## Dashboard Pages

### Page 1 — Gender & Age Group

Highlights structural differences in how men and women participate in the Malaysian labour market.

**Key Metrics (KPI Cards)**
- **Labour Force Participation Rate — Male:** 83%
- **Labour Force Participation Rate — Female:** 56%

**Visuals**

| Visual Type | Title / Description | Fields Used |
|-------------|---------------------|-------------|
| Clustered Column Chart | Salary distribution by gender | `Sheet1.Salary`, `Sheet1.Gender` |
| Bar Chart | Labour force participation rate by age group and gender | `Sex AgeGroup.Age Group`, `Sex AgeGroup.Percentage`, `Sex AgeGroup.Gender` |
| Clustered Column Chart | Average labour force value per gender | `Gender.Gender`, `Gender.Average Value per Gender` |
| 100% Stacked Column Chart | Industry composition by gender (male vs. female share) | `Industry.Industries`, `Industry.Female`, `Industry.Male` |

---

### Page 2 — Ethnic & Education Level

Examines participation disparities across ethnic communities and the relationship between educational attainment and employment outcomes.

**Visuals**

| Visual Type | Title / Description | Fields Used |
|-------------|---------------------|-------------|
| Pie Chart | Labour force share by ethnic group | `Ethnic Groups.Ethnic Groups`, `Ethnic Groups.Value` |
| Clustered Column Chart | Average employment value by educational attainment level | `Education.Educational attainment`, `Education.Average Value` |

---

## Data Sources

| Dataset | Source | Used For |
|---------|--------|----------|
| **2025 Labour Market Review** | [Department of Statistics Malaysia (DOSM)](https://www.dosm.gov.my) | Labour force participation rates, gender breakdown by age group and industry, ethnic group distribution, and educational attainment analysis |
| **Malaysia Salary Data** | [Kaggle — bred54/malaysia-salary-data](https://www.kaggle.com/datasets/bred54/malaysia-salary-data) | Salary distribution analysis by gender (Page 1) |

> All data used in this dashboard is publicly sourced. No proprietary or personally identifiable information is included.

---

## Data Tables (Internal Model)

The Power BI data model contains the following tables:

| Table Name | Description |
|------------|-------------|
| `Sheet1` / `Salary` | Salary records by gender (Kaggle source) |
| `Sex AgeGroup` | Labour force participation rates by gender and age group |
| `Gender` | Aggregated gender-level labour force values |
| `Industry` | Industry-level employment split by male and female |
| `Ethnic Groups` | Labour force participation values by ethnic group |
| `Education` | Employment outcomes by educational attainment level |

---

## Technical Details

| Property | Value |
|----------|-------|
| File format | Power BI Desktop (`.pbix`) |
| Power BI version | 1.28 |
| Report theme | Innovate |
| Number of report pages | 2 |
| Total visuals | 26 (including labels, images, and shapes) |

---

## How to Use

1. Open `DEI_Analysis.pbix` in [Power BI Desktop](https://powerbi.microsoft.com/desktop/).
2. Use the navigation panel on the left side of Page 1 to switch between the **Gender & Age Group** and **Ethnic & Education Level** views.
3. Interact with charts to cross-filter other visuals on the same page.
4. No refresh is needed — the data is embedded in the file.

---

## License & Attribution

This dashboard is built entirely on publicly available data. If you adapt or redistribute this work, please credit the original data sources:

- Department of Statistics Malaysia (DOSM) — [dosm.gov.my](https://www.dosm.gov.my)
- Kaggle dataset by bred54 — [malaysia-salary-data](https://www.kaggle.com/datasets/bred54/malaysia-salary-data)

