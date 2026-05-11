# Diversity, Equity & Inclusion (DEI) Analysis of Employment in Malaysia

A Power BI dashboard exploring workforce participation, salary distribution, and employment composition in Malaysia through the lens of gender, age group, ethnicity, and educational attainment.

---

## 📌 Overview

This dashboard provides a data-driven view of labour market equity in Malaysia. It is structured across two report pages, covering key DEI dimensions using publicly available official and community-sourced datasets.

| Page | Focus Area | Period Covered |
|------|-----------|---------------|
| [Page 1] — Gender & Age Group | Labour force participation rates, salary gaps, industry breakdown | Q2 2022 – Q1 2025 *only salary gaps has no period range* |
| [Page 2] — Ethnic & Education Level | Ethnic group participation, education-level attainment and earnings | Q2 2022 – Q1 2025 |

---

## 📝 Dashboard Pages

### Page 1 — Gender & Age Group

Highlights structural differences in how men and women participate in the Malaysian labour market.

**Key Metrics (KPI Cards)**
- **Labour Force Participation Rate — Male:** 83%
- **Labour Force Participation Rate — Female:** 56%

**Visuals**

| Visual Type | Title / Description | Fields Used |
|-------------|---------------------|-------------|
| Clustered Column Chart | Salary distribution by gender | `Salary.Salary`, `Salary.Gender` |
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
---

## 📊 Dashboard Highlights

The dashboard covers six core DEI dimensions:

| Dimension | What It Analyses |
|---|---|
| **Gender Diversity** | Male vs. female employment rates across sectors and income levels |
| **Ethnicity Breakdown** | Employment distribution across Bumiputera, Chinese, Indian, and other ethnic groups |
| **Age & Generational Diversity** | Workforce composition by age group (Gen Z, Millennial, Gen X, Baby Boomer) |
| **Employment by Sector** | Industry-level employment concentration by demographic group |
| **Salary Equity** | Median salary comparisons across gender, ethnicity, and education level |
| **Educational Attainment** | Relationship between qualification level, employment rate, and earnings |

---

## 🔍 Key Findings

- **Sector concentration by gender**: Women make up approximately 87% of the Activities of households as employers and 66% of Education — while men account for 83% of Agriculture and 90% of Electrical & Construction — indicating that both genders face heavy sector concentration, with women clustered in lower-wage service roles and men in resource sectors.
- **Generational workforce participation**: The 25–34 age group represents the peak of female labour force participation (932), yet this is also where the gap begins to reverse — by 35–44, female participation drops to 879 while male participation rises to 1,158 — pointing to a structural exit from the workforce that coincides with prime family-forming years.
- **Ethnicity and labour force share**: Non-citizens represent the largest single group in Malaysia's labour force at 19.47%, ahead of Bumiputera (15.65%) and all other ethnic groups — highlighting the extent to which the economy depends on migrant labour, a population typically least covered by formal employment protections.
- **Educational attainment impact**: Workers with tertiary education record an average value of 75, compared to 65 for those with no formal education — a 15% difference — yet the gap between tertiary and secondary (SPM-level) qualifications is far narrower at just 75 vs 68, suggesting diminishing returns at the middle education tier.

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| **Microsoft Excel** | Initial data cleaning — manual verification, formatting raw DOSM tables for import |
| **Power BI Desktop** | Dashboard design, data modelling, visual layout, and report publishing |
| **DAX (Data Analysis Expressions)** | Calculated measures and columns — ratios, percentage breakdowns, YoY comparisons, conditional logic |

---

## 📁 Repository Structure

```
dei-malaysia-employment/
│
├── data/
│   ├── raw/                        # Original DOSM datasets (unmodified)
│   └── cleaned/                    # Processed datasets ready for Power BI import
│
├── excel/
│   └── data_prep.xlsx              # Excel data preparation workbook
│
├── powerbi/
│   └── DEI_Malaysia_Dashboard.pbix # Main Power BI dashboard file
│
├── screenshots/
│   └── dashboard_overview page 1.png      # Dashboard preview image
|   └── dashboard_overview page 2.png      # Dashboard preview image 
│
└── README.md
```
---

##  📊 Data Tables (Internal Model)

The Power BI data model contains the following tables:

| Table Name | Description |
|------------|-------------|
| `Salary` | Salary records by gender (Kaggle source) |
| `Sex AgeGroup` | Labour force participation rates by gender and age group |
| `Gender` | Aggregated gender-level labour force values |
| `Industry` | Industry-level employment split by male and female |
| `Ethnic Groups` | Labour force participation values by ethnic group |
| `Education` | Employment outcomes by educational attainment level |

---
## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| **Microsoft Excel** | Initial data cleaning — manual verification, formatting raw DOSM tables for import |
| **Power BI Desktop** | Dashboard design, data modelling, visual layout, and report publishing |
| **DAX (Data Analysis Expressions)** | Calculated measures and columns — ratios, percentage breakdowns, YoY comparisons, conditional logic |

---

## 🖼️ Dashboard Preview

![Dashboard Overview Page 1](DEI%20Malaysia%20Employment/Screenshots/dashboard%20overview%20page%201.jpg)
![Dashboard Overview Page 2](DEI%20Malaysia%20Employment/Screenshots/dashboard%20overview%20page%202.jpg)

---

## 📂 Data Sources

| Dataset | Source | Used For |
|---------|--------|----------|
| **2025 Labour Market Review** | [Department of Statistics Malaysia (DOSM)](https://www.dosm.gov.my) | Labour force participation rates, gender breakdown by age group and industry, ethnic group distribution, and educational attainment analysis |
| **Malaysia Salary Data** | [Kaggle — bred54/malaysia-salary-data](https://www.kaggle.com/datasets/bred54/malaysia-salary-data) | Salary distribution analysis by gender (Page 1) |

> All data used in this dashboard is publicly sourced. No proprietary or personally identifiable information is included.

---

## 💡 Why This Project

Malaysia's workforce equity conversation is growing — driven by government initiatives, ESG reporting requirements, and increasing corporate focus on DEI metrics. Yet much of this data sits in raw government reports that are difficult for HR professionals and business leaders to interpret quickly.

This dashboard was built to answer a simple question: **what does the data actually tell us about who works where, earns what, and why?**

As an HR professional with 17+ years of experience in talent management and workforce operations, I built this project to combine domain knowledge with newly acquired data skills — demonstrating how HR practitioners can use public data to drive more informed, equitable people decisions.

---

## 🚀 How to Use

1. Open `DEI_Malaysia_Dashboard.pbix` in [Power BI Desktop](https://powerbi.microsoft.com/desktop/).
2. Use the navigation panel on the left side of Page 1 to switch between the **Gender & Age Group** and **Ethnic & Education Level** views.
3. Interact with charts to cross-filter other visuals on the same page.
4. No refresh is needed — the data is embedded in the file.

---

## 📬 Connect

**Siti Nurnazihah**
HR Professional transitioning into HR Data Analytics & People Analytics

- 💼 [LinkedIn](https://www.linkedin.com/in/sitinurnazihah)
- 📧 [sitinazihah227@gmail.com]

---

## 📄License & Attribution

This project is open for reference and learning purposes. Data sources belong to DOSM and are subject to their respective usage terms. Please credit this repository if you build upon it.

- Department of Statistics Malaysia (DOSM) — [dosm.gov.my](https://www.dosm.gov.my)
- Kaggle dataset by bred54 — [malaysia-salary-data](https://www.kaggle.com/datasets/bred54/malaysia-salary-data)

---

*Individual student project of Siti Nurnazihah. Built with ♥ as part of an AI & Machine Learning Bootcamp capstone — Nexperts Academy, 2026*
