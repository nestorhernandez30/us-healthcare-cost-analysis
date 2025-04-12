# us-healthcare-cost-analysis
📊 Who Pays More for Healthcare? Exploring U.S. Spending by Income and Insurance Status (MEPS 2019–2022)
A Data Analysis and Visualization Project by Nestor Hernandez

Overview:
This project explores healthcare expenditure patterns across income and insurance groups in the United States using data from the Medical Expenditure Panel Survey (MEPS) for the years 2019–2022. It leverages Python, SQL, and Tableau to clean, analyze, and visualize complex longitudinal data.

📁Key Dashboards (Tableau)

- Pandemic-Era Healthcare Spending
  - Trends in average healthcare expenditures and prescription drug costs during and after the COVID-19 pandemic.

- Spending Differences by Income
  - Breakdown of healthcare costs and out-of-pocket burden by income group.

- ER vs. Hospital Use
  - Utilization patterns by insurance type, highlighting disparities in emergency and inpatient care.

- Income & Insurance Effects on Total Spending
  - Stacked visual showing how both income and insurance shape total healthcare expenditures.

📎 [View the Live Tableau Dashboard](https://public.tableau.com/app/profile/nestor.hernandez7328/viz/WhoPaysMoreforHealthcareExploringU_S_SpendingbyIncomeandInsuranceStatusMEPS2019-2022/Dashboard1#1)

---

🧰 Tools Used

- Python – Data cleaning, imputation, transformation (wide → long), statistical testing
- SQL (SQLite) – Exploratory queries, average and weighted expenditures, group comparisons
- Tableau Public – Data storytelling and visual analytics
- MEPS Data (HC-245) – Longitudinal panel data collected by AHRQ, publicly available [here](https://meps.ahrq.gov/mepsweb/data_stats/download_data_files_detail.jsp?cboPufNumber=HC-245)

---

📁 Methodology Summary

- Data Cleaning: Removed categorical missing values and applied regression + iterative imputation for continuous missing data (hybrid approach).
- Income & Insurance Recoding:
  - Income grouped into 5 bins (Low to High)
  - Insurance grouped into Public, Private, and Uninsured
- Statistical Analysis: Two-sample z-tests for expenditure differences across years, income groups, and insurance groups
- Data Transformation: Converted wide format MEPS data to long format to enable year-level and group-level comparisons.

---
📌 Data & Weighting Notes

Disclaimer:The Medical Expenditure Panel Survey (MEPS) data used in this project is based on a complex survey design intended to produce nationally representative estimates. While some analyses in this project apply survey weights to account for this design, others are unweighted for simplicity and exploratory purposes. SQL and Python outputs use the provided longitudinal weight (`LONGWT`) to compute weighted averages, most visualizations and analyses in this project are exploratory and presented unweighted for clarity and simplicity. Unweighted results may not reflect exact national estimates and should be interpreted with caution. Users should be cautious when interpreting unweighted results, as they may not accurately reflect national estimates.

---

📌 Repository Contents:

- `meps_1922.py` – Full Python script with data cleaning and transformation (with notes intact)
- `MEPS_1922.ipynb` – Jupyter Notebook version with results and outputs included
- `sql_analysis_meps.txt` – Annotated SQL queries with explanations and output results
- `meps19_22_long.csv` – Final long-format dataset (transformed from wide, suitable for SQL & Tableau)

---

License

This project is licensed under the [MIT License](https://opensource.org/licenses/MIT). You are free to use, copy, modify, and distribute this work, but please provide attribution.

---

👤 Author

**Nestor Hernandez** 
Data Analyst | Researcher 
Feel free to connect or reach out!


