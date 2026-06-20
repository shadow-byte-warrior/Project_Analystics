<div align="center">

# 📊 Data Job Market Analysis

### An end-to-end Excel ETL & analytics project

*Exploring salary trends, in-demand skills, and regional pay gaps across data science roles — built on real-world 2023 job posting data.*

[![Excel](https://img.shields.io/badge/Excel-2019%2B-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white)](#-how-to-use)
[![Power Query](https://img.shields.io/badge/Power_Query-ETL-217346?style=for-the-badge&logo=powerautomate&logoColor=white)](#1️⃣-do-more-skills-get-you-better-pay)
[![DAX](https://img.shields.io/badge/DAX-Measures-217346?style=for-the-badge)](#2️⃣-whats-the-salary-for-data-jobs-in-different-regions)

<br/>

[![Stars](https://img.shields.io/github/stars/shadow-byte-warrior/Project_Analystics?style=flat-square&color=2DD4BF)](https://github.com/shadow-byte-warrior/Project_Analystics/stargazers)
[![Forks](https://img.shields.io/github/forks/shadow-byte-warrior/Project_Analystics?style=flat-square&color=2DD4BF)](https://github.com/shadow-byte-warrior/Project_Analystics/network/members)
[![Last Commit](https://img.shields.io/github/last-commit/shadow-byte-warrior/Project_Analystics?style=flat-square&color=2DD4BF)](https://github.com/shadow-byte-warrior/Project_Analystics/commits/main)

</div>

<br/>

<div align="center">

`Extract` → `Transform` → `Model` → `Visualize` → `Insight`

</div>

---

<div align="center">

### 🧭 Explore the analysis

| | | |
|:---:|:---:|:---:|
| 🔍 **[ETL Pipeline](#1️⃣-do-more-skills-get-you-better-pay)** | 🌍 **[Regional Pay](#2️⃣-salary-by-region--pivottables--dax)** | 🛠️ **[Top Skills](#3️⃣-top-skills-of-data-professionals--power-pivot)** |
| 💰 **[Pay by Skill](#4️⃣-pay-for-the-top-10-skills--combo-pivotchart)** | 📋 **[Workbook Structure](#-workbook-structure)** | 💡 **[Key Takeaways](#-key-takeaways)** |

</div>

---

## 📋 Table of Contents

- [Overview](#-overview)
- [Questions Analyzed](#-questions-analyzed)
- [Excel Skills Used](#️-excel-skills-used)
- [Dataset](#-dataset)
- [Analysis Pipeline](#️-analysis-pipeline)
- [Dashboard Highlights](#️-dashboard-highlights)
- [Tools & Tech](#-tools--tech)
- [Analysis Breakdown](#-analysis-breakdown)
- [Workbook Structure](#-workbook-structure)
- [Key Takeaways](#-key-takeaways)
- [How to Use](#-how-to-use)

<br/>

## 📌 Overview

As someone who has navigated the data job market firsthand, I was struck by how little structured data existed to help job seekers understand **what skills to learn** and **what salary to expect**. This project fills that gap.

Using Excel's advanced features — Power Query, Power Pivot, DAX, and Pivot Charts — I analyzed thousands of real job postings to answer four practical questions every data professional should know.

📁 **Dashboard File:** [`1_Project_Analysis.xlsx`](1_Project_Analysis.xlsx)

<br/>

## ❓ Questions Analyzed

| # | Question |
|:---:|---|
| 1️⃣ | Do more skills get you better pay? |
| 2️⃣ | What's the salary for data jobs in different regions? |
| 3️⃣ | What are the top skills of data professionals? |
| 4️⃣ | What's the pay for the top 10 skills? |

<br/>

## 🛠️ Excel Skills Used

| Skill | Purpose |
|---|---|
| 🔍 Power Query (ETL) | Extract, clean, and load job data from raw sources |
| 💪 Power Pivot | Build a relational data model across multiple tables |
| 🧮 DAX | Create custom measures like median salary calculations |
| 📊 Pivot Tables | Slice and dice data across roles, countries, and skills |
| 📈 Pivot Charts | Visualize salary vs. skills with combo charts |

<br/>

## 📂 Dataset

Real-world data science job postings from **2023**, including:

- 👨‍💼 **Job Titles** — Data Analyst, Data Scientist, ML Engineer, Senior Data Engineer, etc.
- 💰 **Salaries** — Annual average in USD
- 📍 **Locations** — US vs. international breakdown
- 🛠️ **Skills** — Required tools and technologies per role

<br/>

## 🏗️ Analysis Pipeline

```mermaid
flowchart LR
    A[(📂 Raw Job\nPostings 2023)] --> B["🔍 Power Query\nExtract · Clean · Load"]
    B --> C["💪 Power Pivot\nData Model (job_id)"]
    C --> D["🧮 DAX Measures\nMedian Salary by Segment"]
    D --> E["📊 Pivot Tables\n& Pivot Charts"]
    E --> F[["💡 Insights\n& Takeaways"]]
```

<br/>

## 🖼️ Dashboard Highlights

<table>
<tr>
<td width="50%"><img src="0_Resources/Images/2_Project_Analysis_Chart1.png" alt="Skills vs Salary" /><p align="center"><sub><strong>Chart 1</strong> — Skills count vs. median salary</sub></p></td>
<td width="50%"><img src="0_Resources/Images/2_Project_Analysis_Chart2.png" alt="US vs Non-US Salary" /><p align="center"><sub><strong>Chart 2</strong> — US vs. Non-US salary by role</sub></p></td>
</tr>
<tr>
<td width="50%"><img src="0_Resources/Images/2_Project_Analysis_Chart3.png" alt="Top Skills" /><p align="center"><sub><strong>Chart 3</strong> — Top 10 skills by likelihood</sub></p></td>
<td width="50%"><img src="0_Resources/Images/2_Project_Analysis_Chart4.png" alt="Pay for Top Skills" /><p align="center"><sub><strong>Chart 4</strong> — Median salary vs. likelihood, top 10 skills</sub></p></td>
</tr>
</table>

<br/>

## 🧰 Tools & Tech

<div align="center">

![Excel](https://img.shields.io/badge/Excel-217346?style=flat-square&logo=microsoftexcel&logoColor=white)
![Power Query](https://img.shields.io/badge/Power_Query-ETL-217346?style=flat-square&logo=powerautomate&logoColor=white)
![Power Pivot](https://img.shields.io/badge/Power_Pivot-Data_Model-217346?style=flat-square)
![DAX](https://img.shields.io/badge/DAX-Measures-217346?style=flat-square)
![Pivot Charts](https://img.shields.io/badge/Pivot_Charts-Combo_%26_Map-217346?style=flat-square)

</div>

<br/>

## 🔍 Analysis Breakdown

<details open>
<summary><strong>1️⃣ Do More Skills Get You Better Pay? — Power Query (ETL)</strong></summary>
<br/>

#### Extract → Transform → Load

Using Power Query, I built two clean queries from the raw dataset:
- `data_jobs_all` — Job-level information (title, salary, country, schedule type)
- `data_job_skills` — Skill-level rows linked by `job_id`

| Step | Action |
|---|---|
| 📥 Extract | Pulled raw data from `data_salary_all.xlsx` |
| 🔄 Transform | Removed unnecessary columns, fixed types, trimmed whitespace, cleaned text |
| 🔗 Load | Loaded both tables into the workbook as structured, analysis-ready tables |

<table>
<tr>
<td><img src="0_Resources/Images/2_Project_Analysis_Screenshot1.png" alt="Power Query Steps - data_jobs_all" /><p align="center"><sub>Applied Steps — <code>data_jobs_all</code></sub></p></td>
<td><img src="0_Resources/Images/2_Project_Analysis_Screenshot2.png" alt="Power Query Steps - data_job_skills" /><p align="center"><sub>Applied Steps — <code>data_job_skills</code></sub></p></td>
</tr>
<tr>
<td><img src="0_Resources/Images/2_Project_Analysis_Screenshot3.png" alt="Power Query Editor - data_jobs_all" /><p align="center"><sub>Loaded Table — <code>data_jobs_all</code></sub></p></td>
<td><img src="0_Resources/Images/2_Project_Analysis_Screenshot4.png" alt="Power Query Editor - data_job_skills" /><p align="center"><sub>Loaded Table — <code>data_job_skills</code></sub></p></td>
</tr>
</table>

**💡 Insight**

![Chart 1 - Skills vs Salary](0_Resources/Images/2_Project_Analysis_Chart1.png)

There is a clear **positive correlation** between the number of skills requested in a job posting and its median salary. Senior Data Engineers (~8.2 skills, ~$150K) and Data Engineers (~7 skills, ~$130K) sit at the top. Business Analysts (~3.3 skills, ~$85K) and Data Analysts (~3.7 skills, ~$90K) are at the lower end.

> **Takeaway:** Every additional relevant skill you build is a measurable lever for higher pay — especially for those targeting Senior or Engineering roles.

</details>

<details>
<summary><strong>2️⃣ Salary by Region — PivotTables + DAX</strong></summary>
<br/>

I created a PivotTable using the Power Pivot data model, then wrote custom DAX measures to compare **US vs. Non-US** median salaries side by side:

```dax
-- Overall Median Salary
Median Salary := MEDIAN(data_jobs_all[salary_year_avg])

-- US-Only Median Salary
US Median Salary :=
CALCULATE(
    MEDIAN(data_jobs_all[salary_year_avg]),
    data_jobs_all[job_country] = "United States"
)
```

**💡 Insight**

![Chart 2 - US vs Non-US Salary PivotTable](0_Resources/Images/2_Project_Analysis_Chart2.png)

Key salary comparisons from the data:

| Role | US Median | Non-US Median |
|---|---|---|
| Senior Data Engineer | $150,000 | $147,500 |
| Machine Learning Engineer | $150,000 | $101,029 |
| Software Engineer | $125,000 | $89,100 |
| Data Engineer | $125,000 | $123,500 |
| Data Scientist | $130,000 | $119,550 |
| Data Analyst | $90,000 | $90,000 |
| Business Analyst | $90,000 | $75,000 |

The US premium is largest for Software Engineers (+$35.9K) and ML Engineers (+$48.9K). Senior Data Engineer salaries are globally competitive — showing strong international demand for that role.

> **Takeaway:** Geography plays a significant role in compensation for most roles. For remote job seekers, targeting US-based companies can be a major salary multiplier.

</details>

<details>
<summary><strong>3️⃣ Top Skills of Data Professionals — Power Pivot</strong></summary>
<br/>

I built a data model in Power Pivot linking `data_jobs_all` and `data_jobs_skill` via the `job_id` foreign key — a **one-to-many** relationship that enables cross-table analysis without VLOOKUP.

<table>
<tr>
<td><img src="0_Resources/Images/2_Project_Analysis_Screenshot5.png" alt="Data Model - Power Pivot" /><p align="center"><sub>Data Model Relationship</sub></p></td>
<td><img src="0_Resources/Images/2_Project_Analysis_Screenshot6.png" alt="Power Pivot Loaded Data" /><p align="center"><sub>Loaded Data in Power Pivot</sub></p></td>
</tr>
</table>

**💡 Insight**

![Chart 3 - Top Skills of Data Professionals](0_Resources/Images/2_Project_Analysis_Chart3.png)

Top 10 skills by likelihood in job postings:

| Rank | Skill | Likelihood |
|:---:|---|---|
| 1 | SQL | ~70% |
| 2 | Python | ~65% |
| 3 | AWS | ~43% |
| 4 | Spark | ~32% |
| 5 | Azure | ~31% |
| 6 | Snowflake | ~25% |
| 7 | Java | ~23% |
| 8 | Hadoop | ~18% |
| 9 | Kafka | ~17% |
| 10 | NoSQL | ~16% |

> **Takeaway:** SQL + Python is the non-negotiable foundation. Cloud platforms (AWS, Azure) and big data tools (Spark, Kafka) are the next layer that separates competitive candidates.

</details>

<details>
<summary><strong>4️⃣ Pay for the Top 10 Skills — Combo PivotChart</strong></summary>
<br/>

I created a combo PivotChart plotting:
- 🟦 **Primary Axis:** Median Salary (clustered column)
- 💠 **Secondary Axis:** Skill Likelihood % (line with diamond markers)

This dual-axis view shows both *how much a skill pays* and *how commonly it's requested* — two very different signals.

**💡 Insight**

![Chart 4 - Pay of Top 10 Skills](0_Resources/Images/2_Project_Analysis_Chart4.png)

| Skill | Median Salary | Likelihood |
|---|---|---|
| Python | ~$98K | ~30% |
| Oracle | ~$95K | ~7% |
| Tableau | ~$95K | ~29% |
| R | ~$93K | ~17% |
| SQL | ~$93K | ~53% |
| Power BI | ~$90K | ~18% |
| SAS | ~$90K | ~19% |
| PowerPoint | ~$85K | ~9% |
| Excel | ~$85K | ~41% |
| Word | ~$82K | ~9% |

SQL is unique — it has the highest likelihood (~53%) AND strong salary (~$93K), making it the single best investment. Python pays the most while remaining highly in demand. PowerPoint and Word trail both in pay and prevalence.

> **Takeaway:** SQL and Python offer the best combination of high pay and high demand. Niche tools like Oracle pay well but appear in fewer postings — useful for specialization after mastering the core stack.

</details>

<br/>

## 📋 Workbook Structure

| Sheet | Contents |
|---|---|
| `Salary_Vs_Skills` | Scatter plot — skills count vs. median salary by role |
| `Salary_Analysis` | PivotTable — US vs. Non-US salary comparison with DAX |
| `Skill_Job_Analysis` | Bar chart — top 10 skills by job posting likelihood |
| `Skill_Salary_Analysis` | Combo chart — median salary + likelihood for top 10 skills |

<br/>

## 💡 Key Takeaways

- 📈 **More skills = more pay** — Senior Data Engineer tops both axes: most skills, highest salary
- 🌍 **US roles pay a premium** — especially for ML Engineers (+$49K) and Software Engineers (+$36K)
- 💻 **SQL is king** — highest demand (~70%) with strong pay (~$93K median)
- 🐍 **Python pays the most** — among top 10 skills, Python leads at ~$98K median
- ☁️ **Cloud is rising** — AWS, Azure, and Spark appear in 30–43% of postings
- 📉 **Office tools don't pay** — PowerPoint and Word rank last in both salary and demand

<br/>

## 🚀 How to Use

1. Download [`1_Project_Analysis.xlsx`](1_Project_Analysis.xlsx)
2. Open in **Microsoft Excel 2019+** (required for Power Query & Power Pivot)
3. Navigate between the **4 analysis sheets** using the bottom tabs
4. Interact with PivotTable filters (country slicer, role dropdown) to explore the data

<br/>

---

<div align="center">

### 👤 Author

**Arun Pandian** — Data Analyst & Data Engineer
📍 Coimbatore, Tamil Nadu, India

[![LinkedIn](https://img.shields.io/badge/-Connect_on_LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/arunpandian-sh2030)
[![GitHub](https://img.shields.io/badge/-shadow--byte--warrior-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/shadow-byte-warrior)

<br/>

### 📄 License

Open for educational and portfolio reference. Dataset sourced from real-world 2023 data science job postings.

<br/>

**[⬆ back to top](#-data-job-market-analysis)**

</div>
