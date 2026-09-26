<div align="center">

# Ayoub El-ouichouany

### Data / Analytics Engineer

📍 Casablanca, Morocco 🇲🇦 · 📞 +212 601 892 215 · ✉️ [ayoub@data-engineer.me](mailto:ayoub@data-engineer.me)

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/ayoub-el-ouichouany/)
[![Portfolio](https://img.shields.io/badge/Portfolio-111827?style=for-the-badge&logo=vercel&logoColor=white)](https://data-engineer.me/)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ayoub-data-analyst)

</div>

<br>

## 👋 About Me

I'm a Data / Analytics Engineer based in Casablanca, Morocco, with hands-on experience turning raw, messy, and large-scale datasets into reliable, analytics-ready information that businesses can actually use to make decisions. My work sits at the intersection of data engineering and analytics engineering: I design and build the pipelines that move data from source systems into a warehouse, I model that data into clean dimensional structures, and I connect it all to dashboards that stakeholders can trust.

My technical foundation covers the full modern data stack — SQL, Python, PostgreSQL, Snowflake, dbt, and Apache Airflow — and I've applied these tools to real, sizeable problems rather than toy datasets. I've worked with 25 million loan applications to understand credit risk, built multi-country real estate data warehouses from scratch with a team, and cleaned and modeled thousands of property listings into star-schema models that power multi-page Power BI dashboards.

What drives me is the belief that good analytics starts with good data engineering. A beautiful dashboard built on inconsistent, untested, or poorly modeled data is a liability, not an asset. That's why I put as much care into data quality testing, referential integrity, and pipeline orchestration as I do into the visualizations at the end of the chain. I like to think of my role as building the plumbing that makes trustworthy decision-making possible — even though nobody sees the pipes, everyone depends on them working.

I'm currently completing a professional Data Analyst training program with CCFBS and Simplon Maghreb, and I hold certifications from Snowflake, LinkedIn Learning, and ALX. I'm comfortable working independently or within a team, following Agile/Scrum practices, and communicating technical concepts to non-technical stakeholders.

### Why Analytics Engineering

I came to this field through a mix of curiosity about numbers and a practical realization: almost every organization sits on more data than it knows what to do with, and the gap between "we have the data" and "we can act on the data" is usually a pipeline problem, not an insight problem. That's the gap I like working in.

Analytics engineering, as a discipline, sits deliberately between data engineering and data analysis. It borrows the rigor of software engineering — version control, testing, modularity, CI/CD — and applies it to the transformation layer that used to live in fragile, undocumented SQL scripts or one-off spreadsheets. Tools like dbt exist precisely because that transformation layer needed the same discipline that application code has had for years: tests, documentation, dependency graphs, and code review. I try to bring that same rigor to every project, even personal ones, because habits built on small projects are the habits that hold up when the data gets bigger and the stakes get higher.

### What I Value in My Work

**Data quality over dashboard polish.** It's tempting to spend most of the time on the visual layer because that's what stakeholders see first. I've learned to resist that pull and put the bulk of my effort into the layers underneath — because a wrong number presented beautifully is still a wrong number, and it's often more dangerous than an obviously ugly one, since people trust it more.

**Reproducibility.** Every pipeline I build should be re-runnable from scratch without manual intervention. If a teammate — or future me — can't rebuild the Gold layer from raw data by just re-running the DAG, then the pipeline isn't actually finished.

**Documentation as part of the deliverable.** dbt's built-in documentation and testing features aren't an afterthought for me; I treat writing tests and descriptions for models as part of the modeling work itself, not a separate task to get around to later.

**Right-sized complexity.** Not every project needs a distributed system or a dozen orchestrated tasks. Part of being a good engineer is matching the complexity of the solution to the complexity of the problem — which is why my smaller projects use simpler tooling (Python, Pandas, PostgreSQL) while my larger ones lean on Snowflake, dbt, and Airflow.

<br>

## 🧭 How I Approach Data Engineering

I follow a consistent methodology across projects, built around the Medallion Architecture pattern:

```
Raw Data → Ingestion → Bronze → Silver → Gold → Dimensional Models → BI / Analytics
```

**Ingestion.** Data is pulled from its source — whether that's a public dataset, an API, or flat files — and landed in its rawest form. Nothing is transformed at this stage; the goal is simply to have a reliable, reproducible copy of the source data.

**Bronze layer.** Raw data is loaded into the warehouse (typically Snowflake or PostgreSQL) with minimal transformation. This layer acts as the single source of truth and the starting point for every downstream transformation, so that if something goes wrong further down the pipeline, I can always rebuild from here.

**Silver layer.** This is where the real cleaning happens: deduplication, type casting, handling of missing values, outlier detection (often via IQR-based methods), and the application of business rules. I treat data quality as a first-class citizen at this stage, writing automated tests to catch anomalies before they propagate further.

**Gold layer.** Cleaned, validated data is modeled into dimensional structures — typically Star Schemas with fact and dimension tables — optimized for analytical queries. This is where I apply dbt heavily, using its testing and documentation features to make the models transparent and maintainable.

**Orchestration.** Apache Airflow ties the whole pipeline together, scheduling and sequencing the movement of data from Bronze to Silver to Gold, with automated retries on failure so pipelines are resilient rather than fragile.

**BI / Analytics.** Finally, the Gold layer connects to Power BI, where I build multi-page dashboards with DAX measures, KPI tracking, and visualizations tailored to the audience — whether that's a business team who needs revenue trends or a risk team who needs a credit-default breakdown.

I've applied this same end-to-end approach across every major project I've built, adapting the specific tools and depth to the scale and nature of the data involved.

<br>

## 🛠️ Technical Skills

**Data Engineering**
ETL/ELT pipeline design, Apache Airflow orchestration, dbt for transformation and testing, SQLAlchemy for Python-to-database connectivity, and automated data quality testing to catch issues before they reach dashboards.

**Data Warehousing & Modeling**
PostgreSQL and Snowflake as warehouse platforms, dimensional data modeling, Star Schema design, and the Medallion Architecture (Bronze/Silver/Gold) as my default approach to structuring pipelines.

**Data Analytics**
Advanced SQL including CTEs and window functions, data cleaning at scale, exploratory data analysis (EDA), and statistical analysis to surface patterns and risk factors in large datasets.

**Business Intelligence**
Power BI as my primary BI tool, DAX for calculated measures, Power Query for data shaping, and Excel for lighter-weight reporting. I focus on KPI reporting and dashboard development that's built to be read by decision-makers, not just data people.

**Programming**
Python as my main language for data work, with Pandas and NumPy for data manipulation and Matplotlib/Seaborn for visualization during the exploratory phase of a project.

**Cloud & DevOps**
Azure Data Factory for cloud-based orchestration, Docker for containerizing pipelines and ensuring reproducibility, and Git/GitHub with GitHub Actions for version control and CI/CD.

**Tools & Ways of Working**
Comfortable working in Agile/Scrum environments, using Jira for sprint planning, backlog management, and task tracking. I value clear communication and documentation as much as clean code.

**Soft Skills**
Autonomy, analytical thinking, problem-solving, rigor, teamwork, technical communication, curiosity, and organization — the traits that, in my experience, matter just as much as the tech stack when a project actually has to ship.

These soft skills show up in concrete ways day to day: autonomy means I can pick up an ambiguous data problem and figure out a reasonable first approach without waiting for every detail to be specified. Rigor means I default to writing a test for a data model even when nobody asked for one, because I'd rather catch a broken assumption myself than have a stakeholder catch it in a live dashboard. Technical communication means translating a Star Schema decision or a dbt incremental strategy into terms a non-technical manager can evaluate and approve, without dumbing down the actual trade-offs involved. And curiosity is what keeps me exploring new parts of the stack — cloud orchestration, CI/CD for data pipelines, more advanced dbt patterns — even outside of what a specific project strictly requires.

<br>

## 🚀 Featured Projects

### 💳 Loan Default Analytics Platform
`Python` `Apache Airflow` `Snowflake` `dbt` `Power BI` `Docker` `GitHub Actions`

This is the largest-scale project I've built, analyzing 25 million loan applications to understand the factors associated with credit risk. Of those 25 million requests, 2.26 million were accepted and 23.23 million were rejected, giving an overall acceptance rate of 8.86%. Within the accepted portfolio, I identified a default rate of 13.03%, corresponding to roughly 294,000 defaulted loans.

To make sense of a dataset this size, I built a full Bronze/Silver/Gold pipeline in Snowflake using dbt, modeling the data into a Star Schema with two fact tables and nine dimension tables. Automated tests were built into the dbt models to check data quality and referential integrity at every layer, so that downstream analysis could be trusted without manual spot-checking.

The pipeline itself runs on a weekly Airflow schedule with four orchestrated tasks, moving data through each layer and triggering the dbt transformations in sequence. On top of the Gold layer, I built a five-page Power BI dashboard covering credit risk indicators, customer profiles, and overall financial performance of the loan portfolio — giving stakeholders a way to explore both the "who" and the "why" behind loan defaults.

This project pushed me to think seriously about performance at scale: query optimization, efficient dbt materializations, and pipeline reliability all became genuinely important rather than theoretical concerns once the row counts hit the tens of millions.

**Key challenges and how I approached them:** At this scale, naive transformations that work fine on a few thousand rows can quietly become the slowest part of the entire pipeline. I had to think carefully about which dbt models should be materialized as tables versus views, where incremental models made sense to avoid reprocessing the full 25 million rows on every run, and how to structure the fact and dimension tables so that the most common queries — risk breakdowns by customer segment, trends over time — stayed fast. The nine-dimension model reflects a deliberate choice to normalize shared attributes (customer demographics, loan terms, time, geography, and more) rather than flattening everything into a single wide table, which kept the Gold layer both queryable and maintainable.

**What I learned:** Working with a dataset this size taught me that data quality testing isn't optional at scale — it's the only way to catch a broken join or a duplicated row before it silently inflates a KPI by a few percentage points and nobody notices until a stakeholder asks an uncomfortable question in a meeting.

### 🏠 Real Estate Data Warehouse
*(Group project, team of 4)*
`Snowflake` `dbt` `Apache Airflow` `Power BI` `Docker`

Working as part of a four-person team, I helped design and build a multi-country real estate data warehouse integrating 2,060 property listings. We used Snowflake as the warehouse platform, dbt for transformation, a Medallion Bronze/Silver/Gold architecture, and a Star Schema model, with the Gold layer connected directly to Power BI for reporting.

My contribution included industrializing and orchestrating a five-task Apache Airflow DAG that automated the loading of the Bronze layer, ran the dbt transformations, and executed tests on the Silver and Gold layers — with automatic recovery in case of failure, so the pipeline didn't require manual intervention every time something hiccuped.

The final output was a three-page Power BI dashboard connected to the Gold layer, allowing analysis of prices, property characteristics, and trends by country. Among the findings: France represented 23% of all listings, and houses made up 23.1% of the properties analyzed. Working in a team on this project also gave me experience coordinating data modeling decisions across multiple contributors — agreeing on schema design, naming conventions, and testing standards so the pipeline stayed coherent as more people touched it.

**Team dynamics:** Building this warehouse with three other people meant that "it works on my machine" wasn't good enough — every model, DAG task, and test had to be understandable and runnable by teammates who hadn't necessarily written that specific piece. We split responsibilities across the pipeline (ingestion, transformation, orchestration, and reporting), which meant clear interface contracts between layers mattered as much as the internal logic of any one layer. This is where the automatic recovery logic in the Airflow DAG came from directly — with four people committing changes, something breaking mid-pipeline was a "when," not an "if," and manual re-triggering wasn't a scalable answer.

**Data storytelling:** Beyond the technical build, this project sharpened how I think about presenting findings. The France-23%-of-listings and houses-23.1%-of-properties figures aren't just numbers on a dashboard — they're the kind of detail a stakeholder can use directly to decide where to focus a marketing budget or which markets need more listing coverage. I try to design dashboards around the decisions they're meant to support, not just around the data that happens to be available.

### 🏡 Darkom Real Estate Analytics Platform
`Python` `Pandas` `PostgreSQL` `SQLAlchemy` `Power BI`

This project focused on 1,508 real estate listings spread across 10 Moroccan cities, with the goal of understanding property distribution and pricing trends in the local market. I used Python and Pandas for the analysis layer and PostgreSQL as the underlying database, connected via SQLAlchemy.

A major part of this project was data cleaning: after treating missing values, inconsistencies, and outliers — using contextual imputation, IQR-based outlier detection, and business-rule validation — I retained 95.9% of the original records, which I consider a strong result given how messy real-world listing data tends to be.

From there, I designed a Star Schema with one fact table and four dimensions, and enriched the dataset with seven derived variables to support deeper analysis. The final deliverable was a four-page Power BI dashboard, which revealed that apartments represented 49% of all listings, while villas had the highest average prices of any property type. This project was a good exercise in doing rigorous data engineering even at a smaller scale — the cleaning and modeling discipline doesn't change just because the dataset is a few thousand rows instead of millions.

**On the cleaning process specifically:** Real estate listing data scraped or aggregated from multiple sources is notoriously inconsistent — missing square footage, inconsistent city naming, prices entered in different currencies or formats, and outlier listings that are either data-entry errors or genuinely unusual properties. Rather than dropping every incomplete row, which would have thrown away a meaningful chunk of the dataset, I used contextual imputation (filling gaps based on similar listings in the same city and property type), IQR-based statistical methods to flag genuine outliers versus normal variation, and business rules to catch impossible values (like a studio apartment listed with five bedrooms). That combination is what got retention up to 95.9% while still keeping the resulting dataset trustworthy.

**Why the derived variables mattered:** The seven derived variables I added — things like price per square meter and normalized location tiers — weren't just for show. They're what made the dashboard able to answer comparative questions ("is this villa overpriced for its city?") rather than just descriptive ones ("how many villas are there?"). That distinction, between a dashboard that describes data and one that supports a decision, is something I actively design for in every project.

<br>

## 🎓 Education & Certifications

**Professional Training – Data Analyst**
CCFBS × Simplon Maghreb, Fquih Ben Salah — January 2026 to August 2026

**Baccalauréat – Economic Sciences**
Lycée Technique El Khawarezmi, Souk Sebt Ouled Nemma — 2025

**Certifications:**
- Data Engineering Professional Certificate – Snowflake (2026)
- SQL Essential Training – LinkedIn Learning (2026)
- Power BI Essential Training – LinkedIn Learning (2026)
- AI Career Essentials (AICE) – ALX (September–November 2024)

<br>

## 🌍 Languages

- **Arabic** — Native
- **French** — Technical/professional communication
- **English** — Technical/professional communication

<br>

## 🎯 What I'm Looking For

I'm looking to grow as a Data or Analytics Engineer within a team where I can keep building end-to-end pipelines — from raw ingestion through to the dashboards decision-makers actually use. I'm particularly drawn to roles that combine SQL-heavy transformation work with dbt and cloud data warehouses, and where data quality and testing are treated as seriously as the analysis built on top of them.

I'm equally comfortable owning a project from scratch, as I did with the Darkom platform, or plugging into an existing pipeline and improving it — adding tests, refactoring inefficient models, or extending orchestration to cover edge cases nobody had gotten around to handling yet. I enjoy the kind of work where you can point at a dashboard and know, with confidence, exactly which raw table and which transformation produced every number on it.

If you're working on a data problem — whether it's a messy dataset, a pipeline that needs to scale, or a reporting layer that nobody quite trusts yet — I'd be glad to talk about it. I'm also happy to walk through the technical decisions behind any of the projects above in more depth — the trade-offs I made, what I'd do differently now, and how the same approach could apply to a different domain or dataset.

<br>

## 📫 Let's Connect

I'm always open to talking data engineering, analytics, or potential collaborations. Whether you're looking at a pipeline design problem, a messy dataset that needs taming, or a dashboard that needs to actually answer the right questions — feel free to reach out.

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/ayoub-el-ouichouany/)
[![Portfolio](https://img.shields.io/badge/Portfolio-111827?style=for-the-badge&logo=vercel&logoColor=white)](https://data-engineer.me/)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ayoub-data-analyst)
[![Email](https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:ayoub@data-engineer.me)

</div>
