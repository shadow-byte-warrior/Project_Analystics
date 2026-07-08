<div align="center">

# 📊 DATA SCIENCE JOB MARKET — ANALYTICS DASHBOARD
### Excel-Powered Salary & Skills Intelligence

<img src="https://img.shields.io/badge/STATUS-LIVE-brightgreen?style=for-the-badge&labelColor=1a1a2e" />
<img src="https://img.shields.io/badge/DATA_YEAR-2023-blue?style=for-the-badge&labelColor=1a1a2e" />
<img src="https://img.shields.io/badge/RECORDS-Thousands_of_Postings-orange?style=for-the-badge&labelColor=1a1a2e" />

<br/>

![Excel](https://img.shields.io/badge/Microsoft_Excel-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white)
![Power Query](https://img.shields.io/badge/Power_Query-ETL-2C5E1A?style=for-the-badge)
![Power Pivot](https://img.shields.io/badge/Power_Pivot-DAX-yellow?style=for-the-badge&logoColor=black)
![License](https://img.shields.io/badge/License-Educational-blue?style=for-the-badge)

![Stars](https://img.shields.io/github/stars/shadow-byte-warrior/Project_Analystics?style=flat-square&label=STARS&color=gold)
![Forks](https://img.shields.io/github/forks/shadow-byte-warrior/Project_Analystics?style=flat-square&label=FORKS)
![Last Commit](https://img.shields.io/github/last-commit/shadow-byte-warrior/Project_Analystics?style=flat-square&label=LAST%20UPDATE)

*A real-world Excel dashboard decoding salary trends, in-demand skills, and regional pay gaps across data careers — built with Power Query, Power Pivot, and DAX.*

<br/>

**[📥 Download the Workbook](https://github.com/shadow-byte-warrior/Project_Analystics/blob/main/1_Project_Analysis.xlsx)** &nbsp;·&nbsp; **[⭐ Star this Repo](https://github.com/shadow-byte-warrior/Project_Analystics)**

</div>

<br/>

---

<div align="center">

### 🎛️ QUICK-GLANCE KPI STRIP

| 💼 Top Paying Role | 🔥 Highest US Premium | 🧠 #1 In-Demand Skill | 💰 Highest-Paying Skill |
|:---:|:---:|:---:|:---:|
| **Senior Data Engineer**<br/>`$150,000` | **ML Engineer**<br/>`+$48.9K` | **SQL**<br/>`~70% of postings` | **Python**<br/>`~$98K median` |

</div>

---

## 🗂️ Dashboard Navigation

<table align="center">
<tr>
<td align="center" width="20%"><a href="#-mission-briefing">🎯<br/><b>Mission<br/>Briefing</b></a></td>
<td align="center" width="20%"><a href="#-the-four-questions">❓<br/><b>Questions<br/>Analyzed</b></a></td>
<td align="center" width="20%"><a href="#️-tech-stack--pipeline">🛠️<br/><b>Tech Stack<br/>& Pipeline</b></a></td>
<td align="center" width="20%"><a href="#-panel-01--skills-vs-pay">📊<br/><b>Analysis<br/>Panels</b></a></td>
<td align="center" width="20%"><a href="#-key-takeaways-board">💡<br/><b>Takeaways<br/>Board</b></a></td>
</tr>
</table>

---

## 🎯 Mission Briefing

As someone who's navigated the data job market firsthand, I noticed a gap: very little structured data exists to help job seekers know **what skills to learn** and **what salary to realistically expect**.

This dashboard closes that gap — turning thousands of raw 2023 job postings into four decision-ready answers using nothing but Excel's advanced analytics toolkit.

<div align="center">

```mermaid
flowchart LR
    A["📥 Raw Job Postings\n2023 Dataset"] --> B["🔍 Power Query\nExtract · Clean · Transform"]
    B --> C["💪 Power Pivot\nData Model"]
    C --> D["🧮 DAX Measures\nMedian Salary · US vs Non-US"]
    D --> E["📊 PivotTables\n& PivotCharts"]
    E --> F["💡 Insights\n& Takeaways"]

    style A fill:#1a1a2e,stroke:#e94560,color:#fff
    style B fill:#16213e,stroke:#0f3460,color:#fff
    style C fill:#0f3460,stroke:#e94560,color:#fff
    style D fill:#16213e,stroke:#0f3460,color:#fff
    style E fill:#1a1a2e,stroke:#e94560,color:#fff
    style F fill:#e94560,stroke:#1a1a2e,color:#fff
```

</div>

<details>
<summary><b>📂 About the Dataset (click to expand)</b></summary>
<br/>

Real-world data science job postings from **2023**, including:

| Field | Description |
|---|---|
| 👨‍💼 **Job Titles** | Data Analyst, Data Scientist, ML Engineer, Senior Data Engineer, etc. |
| 💰 **Salaries** | Annual average in USD |
| 📍 **Locations** | US vs. international breakdown |
| 🛠️ **Skills** | Required tools and technologies per role |

</details>

---

## ❓ The Four Questions

<div align="center">

| # | Question | Panel |
|:---:|---|:---:|
| 1️⃣ | Do more skills get you better pay? | [`→ Panel 01`](#-panel-01--skills-vs-pay) |
| 2️⃣ | What's the salary for data jobs across regions? | [`→ Panel 02`](#-panel-02--regional-salary-radar) |
| 3️⃣ | What are the top skills of data professionals? | [`→ Panel 03`](#-panel-03--skill-leaderboard) |
| 4️⃣ | What's the pay for the top 10 skills? | [`→ Panel 04`](#-panel-04--pay-vs-demand-matrix) |

</div>

---

## 🛠️ Tech Stack & Pipeline

<div align="center">

| Skill | Purpose |
|:---:|---|
| 🔍 **Power Query (ETL)** | Extract, clean, and load job data from raw sources |
| 💪 **Power Pivot** | Build a relational data model across multiple tables |
| 🧮 **DAX** | Custom measures — e.g. median salary, US vs. Non-US splits |
| 📊 **Pivot Tables** | Slice and dice data across roles, countries, and skills |
| 📈 **Pivot Charts** | Combo visualizations — salary vs. skills, dual-axis views |

</div>

---

## 📊 Panel 01 — Skills vs. Pay

**Excel Skill:** `Power Query (ETL)`

<details open>
<summary><b>🔍 Extract → Transform → Load</b></summary>
<br/>

Two clean queries were built from the raw dataset:

- `data_jobs_all` — job-level info (title, salary, country, schedule type)
- `data_job_skills` — skill-level rows linked by `job_id`

| Step | Action |
|:---:|---|
| 📥 Extract | Pulled raw data from `data_salary_all.xlsx` |
| 🔄 Transform | Removed unnecessary columns, fixed types, trimmed whitespace, cleaned text |
| 🔗 Load | Loaded both tables as structured, analysis-ready tables |

<table>
<tr>
<td width="50%" align="center"><b>Applied Steps — <code>data_jobs_all</code></b><br/><br/>
<a href="https://github.com/shadow-byte-warrior/Project_Analystics/blob/main/0_Resources/Images/2_Project_Analysis_Screenshot1.png"><img src="https://github.com/shadow-byte-warrior/Project_Analystics/raw/main/0_Resources/Images/2_Project_Analysis_Screenshot1.png" width="100%"/></a>
</td>
<td width="50%" align="center"><b>Applied Steps — <code>data_job_skills</code></b><br/><br/>
<a href="https://github.com/shadow-byte-warrior/Project_Analystics/blob/main/0_Resources/Images/2_Project_Analysis_Screenshot2.png"><img src="https://github.com/shadow-byte-warrior/Project_Analystics/raw/main/0_Resources/Images/2_Project_Analysis_Screenshot2.png" width="100%"/></a>
</td>
</tr>
<tr>
<td width="50%" align="center"><b>Loaded Table — <code>data_jobs_all</code></b><br/><br/>
<a href="https://github.com/shadow-byte-warrior/Project_Analystics/blob/main/0_Resources/Images/2_Project_Analysis_Screenshot3.png"><img src="https://github.com/shadow-byte-warrior/Project_Analystics/raw/main/0_Resources/Images/2_Project_Analysis_Screenshot3.png" width="100%"/></a>
</td>
<td width="50%" align="center"><b>Loaded Table — <code>data_job_skills</code></b><br/><br/>
<a href="https://github.com/shadow-byte-warrior/Project_Analystics/blob/main/0_Resources/Images/2_Project_Analysis_Screenshot4.png"><img src="https://github.com/shadow-byte-warrior/Project_Analystics/raw/main/0_Resources/Images/2_Project_Analysis_Screenshot4.png" width="100%"/></a>
</td>
</tr>
</table>
</details>

<div align="center">

[![Chart 1 - Skills vs Salary](https://github.com/shadow-byte-warrior/Project_Analystics/raw/main/0_Resources/Images/2_Project_Analysis_Chart1.png)](https://github.com/shadow-byte-warrior/Project_Analystics/blob/main/0_Resources/Images/2_Project_Analysis_Chart1.png)

</div>

> #### 💡 Insight
> There's a clear **positive correlation** between the number of skills a job posting requires and its median salary. **Senior Data Engineers** (~8.2 skills, ~$150K) and **Data Engineers** (~7 skills, ~$130K) top the chart. **Business Analysts** (~3.3 skills, ~$85K) and **Data Analysts** (~3.7 skills, ~$90K) sit lower.
>
> 🎯 **Takeaway:** Every additional relevant skill is a measurable lever for higher pay — especially for Senior or Engineering-track roles.

<div align="right">

[`↑ Back to nav`](#️-dashboard-navigation)

</div>

---

## 📊 Panel 02 — Regional Salary Radar

**Excel Skills:** `PivotTables` + `DAX`

A PivotTable built on the Power Pivot data model, driven by custom DAX measures comparing **US vs. Non-US** medians:

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

<div align="center">

[![Chart 2 - US vs Non-US Salary PivotTable](https://github.com/shadow-byte-warrior/Project_Analystics/raw/main/0_Resources/Images/2_Project_Analysis_Chart2.png)](https://github.com/shadow-byte-warrior/Project_Analystics/blob/main/0_Resources/Images/2_Project_Analysis_Chart2.png)

</div>

<div align="center">

| Role | 🇺🇸 US Median | 🌍 Non-US Median | US Premium |
|---|---:|---:|:---:|
| Senior Data Engineer | $150,000 | $147,500 | +$2.5K |
| Machine Learning Engineer | $150,000 | $101,029 | 🔥 +$48.9K |
| Software Engineer | $125,000 | $89,100 | 🔥 +$35.9K |
| Data Engineer | $125,000 | $123,500 | +$1.5K |
| Data Scientist | $130,000 | $119,550 | +$10.5K |
| Data Analyst | $90,000 | $90,000 | — |
| Business Analyst | $90,000 | $75,000 | +$15K |

</div>

> #### 💡 Insight
> The US premium is largest for **Software Engineers** (+$35.9K) and **ML Engineers** (+$48.9K). Senior Data Engineer pay is globally competitive, signaling strong international demand for that role.
>
> 🎯 **Takeaway:** Geography materially affects compensation for most roles. Remote job seekers targeting US-based companies can unlock a significant salary multiplier.

<div align="right">

[`↑ Back to nav`](#️-dashboard-navigation)

</div>

---

## 📊 Panel 03 — Skill Leaderboard

**Excel Skill:** `Power Pivot (Data Modeling)`

A data model links `data_jobs_all` and `data_jobs_skill` via the `job_id` foreign key — a **one-to-many** relationship enabling cross-table analysis without VLOOKUP.

<details>
<summary><b>🔗 View Data Model & Loaded Tables</b></summary>
<br/>

<div align="center">

**Data Model Relationship**

[![Data Model - Power Pivot](https://github.com/shadow-byte-warrior/Project_Analystics/raw/main/0_Resources/Images/2_Project_Analysis_Screenshot5.png)](https://github.com/shadow-byte-warrior/Project_Analystics/blob/main/0_Resources/Images/2_Project_Analysis_Screenshot5.png)

**Loaded Data in Power Pivot**

[![Power Pivot Loaded Data](https://github.com/shadow-byte-warrior/Project_Analystics/raw/main/0_Resources/Images/2_Project_Analysis_Screenshot6.png)](https://github.com/shadow-byte-warrior/Project_Analystics/blob/main/0_Resources/Images/2_Project_Analysis_Screenshot6.png)

</div>
</details>

<div align="center">

[![Chart 3 - Top Skills of Data Professionals](https://github.com/shadow-byte-warrior/Project_Analystics/raw/main/0_Resources/Images/2_Project_Analysis_Chart3.png)](https://github.com/shadow-byte-warrior/Project_Analystics/blob/main/0_Resources/Images/2_Project_Analysis_Chart3.png)

| Rank | Skill | Likelihood |
|:---:|---|---|
| 🥇 1 | 🐘 SQL | `███████░` ~70% |
| 🥈 2 | 🐍 Python | `██████░░` ~65% |
| 🥉 3 | ☁️ AWS | `████░░░░` ~43% |
| 4 | ⚡ Spark | `███░░░░░` ~32% |
| 5 | ☁️ Azure | `███░░░░░` ~31% |
| 6 | ❄️ Snowflake | `██░░░░░░` ~25% |
| 7 | ☕ Java | `██░░░░░░` ~23% |
| 8 | 🐘 Hadoop | `██░░░░░░` ~18% |
| 9 | 📨 Kafka | `█░░░░░░░` ~17% |
| 10 | 🗄️ NoSQL | `█░░░░░░░` ~16% |

</div>

> #### 💡 Insight
> SQL + Python form the non-negotiable foundation. Cloud platforms (AWS, Azure) and big data tools (Spark, Kafka) are the next layer separating competitive candidates.
>
> 🎯 **Takeaway:** Master SQL and Python first — then layer in one cloud platform and one big-data tool to stand out.

<div align="right">

[`↑ Back to nav`](#️-dashboard-navigation)

</div>

---

## 📊 Panel 04 — Pay vs. Demand Matrix

**Excel Skill:** `Advanced Combo PivotChart`

A combo PivotChart plotting:

- 🟦 **Primary Axis** — Median Salary (clustered column)
- 💠 **Secondary Axis** — Skill Likelihood % (line with diamond markers)

This dual-axis view separates *how much a skill pays* from *how often it's requested* — two very different signals.

<div align="center">

[![Chart 4 - Pay of Top 10 Skills](https://github.com/shadow-byte-warrior/Project_Analystics/raw/main/0_Resources/Images/2_Project_Analysis_Chart4.png)](https://github.com/shadow-byte-warrior/Project_Analystics/blob/main/0_Resources/Images/2_Project_Analysis_Chart4.png)

| Skill | Median Salary | Likelihood |
|---|---:|---:|
| 🐍 Python | ~$98K | ~30% |
| 🗄️ Oracle | ~$95K | ~7% |
| 📊 Tableau | ~$95K | ~29% |
| 📈 R | ~$93K | ~17% |
| 🐘 SQL | ~$93K | ~53% |
| 📊 Power BI | ~$90K | ~18% |
| 📉 SAS | ~$90K | ~19% |
| 📽️ PowerPoint | ~$85K | ~9% |
| 📗 Excel | ~$85K | ~41% |
| 📝 Word | ~$82K | ~9% |

</div>

> #### 💡 Insight
> SQL is unique — highest likelihood (~53%) **and** strong salary (~$93K), making it the single best investment. Python pays the most while staying highly in demand. PowerPoint and Word trail on both fronts.
>
> 🎯 **Takeaway:** SQL and Python offer the best pay-to-demand ratio. Niche tools like Oracle pay well but appear less often — good for specialization *after* the core stack.

<div align="right">

[`↑ Back to nav`](#️-dashboard-navigation)

</div>

---

## 📋 Workbook Structure

<div align="center">

| Sheet | Contents |
|---|---|
| `Salary_Vs_Skills` | Scatter plot — skills count vs. median salary by role |
| `Salary_Analysis` | PivotTable — US vs. Non-US salary comparison with DAX |
| `Skill_Job_Analysis` | Bar chart — top 10 skills by job posting likelihood |
| `Skill_Salary_Analysis` | Combo chart — median salary + likelihood for top 10 skills |

</div>

---

## 💡 Key Takeaways Board

<div align="center">

| 📈 More Skills = More Pay | 🌍 US Roles Pay a Premium | 💻 SQL Is King |
|:---:|:---:|:---:|
| Senior Data Engineer tops both axes | Especially ML Engineers (+$49K) & SWE (+$36K) | ~70% demand, ~$93K median |

| 🐍 Python Pays the Most | ☁️ Cloud Is Rising | 📉 Office Tools Don't Pay |
|:---:|:---:|:---:|
| ~$98K median among top 10 skills | AWS/Azure/Spark in 30–43% of postings | PowerPoint & Word rank last |

</div>

---

## 🚀 How to Use

1. Download [`1_Project_Analysis.xlsx`](https://github.com/shadow-byte-warrior/Project_Analystics/blob/main/1_Project_Analysis.xlsx)
2. Open in **Microsoft Excel 2019+** (required for Power Query & Power Pivot)
3. Navigate the **4 analysis sheets** via the bottom tabs
4. Use PivotTable filters (country slicer, role dropdown) to explore the data live

---

<div align="center">

## 👤 Author

**Arun Pandian**
AI & Data Science Graduate · Aspiring Data Analyst
📍 Coimbatore, Tamil Nadu, India

[![LinkedIn](https://img.shields.io/badge/LinkedIn-arunpandiansh2030-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/arunpandiansh2030)
[![GitHub](https://img.shields.io/badge/GitHub-shadow--byte--warrior-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/shadow-byte-warrior)

---

### 📄 License

Open for educational and portfolio reference. Dataset sourced from real-world 2023 data science job postings.

⭐ **If this dashboard helped you understand the data job market, consider giving it a star!**

</div>
