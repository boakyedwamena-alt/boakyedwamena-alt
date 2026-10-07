<h1 align="center">Hi, I'm Emmanuel 👋</h1>
<h3 align="center">Data Analyst · Data Science · BI · Python · SQL · Machine Learning</h3>

<p align="center">
  <a href="https://linkedin.com/in/emmanuel-dwamena">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white" alt="LinkedIn"/>
  </a>
  <a href="https://tally.so/r/xXex1d">
    <img src="https://img.shields.io/badge/Contact%20Form-D14836?style=flat&logo=gmail&logoColor=white" alt="Contact form"/>
  </a>
  <img src="https://img.shields.io/badge/London%2C%20UK-000000?style=flat&logo=googlemaps&logoColor=white" alt="Location"/>
</p>

---

### 👤 About Me

I'm a recent MSc Data Analytics graduate with a Biomedical Science background, based in London. I turn messy data into clear answers: cleaning and modelling it in Python and SQL, building machine learning models I can explain and test honestly, and presenting results in Tableau dashboards that non-technical people can use.

My portfolio here covers a machine learning pipeline with SHAP interpretability, a Tableau sales dashboard built on ~100,000 orders, SQL analysis on BigQuery, and an end-to-end data engineering pipeline (PostgreSQL, dbt, Airflow, Docker) on 12.5 million taxi trips. My science background means I'm careful about data quality, uncertainty and what the numbers can and can't support, which matters most in healthcare and clinical analytics.

I'm looking for data analyst, BI, reporting or junior data scientist roles in London or remote, and I'm open to opportunities across industries.

- 🎓 MSc Data Analytics (Distinction), University of Portsmouth
- 🔬 BSc (Hons) Biomedical Science, University of Portsmouth
- 🌱 Actively adding new projects to this portfolio
- 💬 Ask me about machine learning pipelines, SHAP interpretability, SQL analysis, Tableau dashboards or data pipelines with dbt and Airflow
- 📫 Best way to reach me: [LinkedIn](https://linkedin.com/in/emmanuel-dwamena) or the contact form above

---

### 🛠️ Tech Stack

<table>
  <tr>
    <td><b>Languages &amp; Querying</b></td>
    <td>
      <img src="https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white"/>
      <img src="https://img.shields.io/badge/SQL-4479A1?style=flat&logo=postgresql&logoColor=white"/>
      <img src="https://img.shields.io/badge/BigQuery-669DF6?style=flat&logo=googlebigquery&logoColor=white"/>
      <img src="https://img.shields.io/badge/R-276DC3?style=flat&logo=r&logoColor=white"/>
    </td>
  </tr>
  <tr>
    <td><b>Analytics &amp; BI</b></td>
    <td>
      <img src="https://img.shields.io/badge/Tableau-E97627?style=flat&logo=tableau&logoColor=white"/>
      <img src="https://img.shields.io/badge/Power%20BI-F2C811?style=flat&logo=powerbi&logoColor=black"/>
      <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white"/>
      <img src="https://img.shields.io/badge/Excel-217346?style=flat&logo=microsoftexcel&logoColor=white"/>
      <img src="https://img.shields.io/badge/SPSS-1E88E5?style=flat"/>
    </td>
  </tr>
  <tr>
    <td><b>Machine Learning &amp; Data</b></td>
    <td>
      <img src="https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white"/>
      <img src="https://img.shields.io/badge/NumPy-013243?style=flat&logo=numpy&logoColor=white"/>
      <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=flat&logo=scikitlearn&logoColor=white"/>
      <img src="https://img.shields.io/badge/XGBoost-337AB7?style=flat"/>
      <img src="https://img.shields.io/badge/KNIME-FFCC00?style=flat"/>
    </td>
  </tr>
   <tr>
    <td><b>Data Engineering</b></td>
    <td>
      <img src="https://img.shields.io/badge/dbt-FF694B?style=flat&logo=dbt&logoColor=white"/>
      <img src="https://img.shields.io/badge/Airflow-017CEE?style=flat&logo=apacheairflow&logoColor=white"/>
      <img src="https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white"/>
      <img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat&logo=githubactions&logoColor=white"/>
    </td>
  </tr>
</table>

---

### 🚀 Featured Projects

#### 🚕 [NYC Taxi Data Engineering Pipeline](https://github.com/boakyedwamena-alt/nyc-taxi-data-pipeline)
*Data engineering project · PostgreSQL, dbt, Airflow, Docker*
An end-to-end ELT pipeline that loads 12.5 million NYC yellow taxi trips and hourly weather data into PostgreSQL, models them into a tested star schema, and serves the results in a Streamlit dashboard.
- Built idempotent Python ingestion into a month-partitioned raw layer, dbt staging and incremental fact models with 27 data tests, and an Airflow DAG, all running in Docker with GitHub Actions CI
- Cut a one-day query from about 16 s to under 0.3 s with a B-tree index (single run on an 8 GB laptop), and a 1.7 s aggregation to 0.18 ms with a materialized view; benchmarks and their limits are documented in the repo
- Flagged about 3.8% of raw rows as invalid instead of silently dropping them, and found weekday demand peaking at 6 pm and fewer trips in freezing hours, while noting that four months of data and a single weather point cannot show cause

`Python` `PostgreSQL` `dbt` `Airflow` `Docker` `SQL`




#### 🩺 [Diabetes Risk Classification — Machine Learning Pipeline](https://github.com/boakyedwamena-alt/diabetes-risk-pipeline)
*Machine learning project*
An end-to-end ML pipeline on the Pima Indians Diabetes dataset, following TRIPOD reporting guidance and combining a biomedical science background with applied machine learning.
- Built leakage-safe preprocessing (training-set-only imputation, outlier capping and scaling), five tuned base classifiers with 5-fold cross-validation and ADASYN class balancing, and a stacking ensemble
- Stacking ensemble caught 41 of 54 diabetic patients in the held-out test set (recall 0.76) versus 38 for a plain logistic regression baseline; bootstrap confidence intervals show the gain is not statistically clear on a test set this small, and the README reports that openly
- Used SHAP values and partial dependence plots to show glucose, BMI and insulin drive the predictions

`Python` `scikit-learn` `XGBoost` `SHAP` `Machine Learning`

#### 📊 [Olist Brazilian E-Commerce Sales Dashboard](https://github.com/boakyedwamena-alt/olist-sales-dashboard)
*Tableau · [Live dashboard](https://public.tableau.com/views/OlistSalesPerformancceDashboard/OlistSalesPerformanceDashboard?:language=en-GB&:display_count=n&:origin=viz_share_link)*
An interactive dashboard analysing ~100,000 orders from a Brazilian marketplace, covering sales trends, product categories, delivery performance, reviews and geography.
- Modelled nine relational tables in Tableau using relationships to avoid row duplication, and documented every data-cleaning fix (hidden BOM character, 1M-row geolocation table reduced to one row per zip code)
- Surfaced insights such as revenue concentrated in two categories and Southeast Brazil, and a long tail of slow deliveries as the clearest operational opportunity

`Tableau` `Excel` `Data Cleaning` `Dashboard Design`

#### 🔎 [Stack Overflow SQL Analysis](https://github.com/boakyedwamena-alt/stackoverflow-sql-analysis)
*Google BigQuery*
Three documented SQL queries on the public Stack Overflow dataset, looking at how community activity, interests and responsiveness changed over time.
- Showed Python's share of questions rising from about 4% (2012) to 16% (2021) and overtaking JavaScript in 2019, using shares rather than raw counts to handle partial years
- Used window functions, CTEs, array unnesting, conditional aggregation and approximate medians, with notes on query cost and the limits of the analysis

`SQL` `BigQuery` `Window Functions` `Data Analysis`

---

### 📊 GitHub Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=boakyedwamena-alt&show_icons=true&theme=default&count_private=true" alt="GitHub Stats" height="165"/>
</p>

---

<p align="center"><i>Open to Data Analyst, BI and Data Science roles in London and remote.</i></p>
