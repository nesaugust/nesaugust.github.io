# Agnes Jeni Makay | Data Analytics Portfolio

I'm a data analyst and statistician based in Sydney, with over five years of experience in official statistics and a Master of Data Science and Decisions from UNSW. My projects cover data preparation, business reporting, predictive modelling and LLM evaluation.

I’m currently a Data Scientist and Product Analyst Intern at ORison Tech, where I evaluate LLM outputs, check the quality of AI-generated analyses, and contribute to dashboard design and product requirements.

[Visit the portfolio](https://nesaugust.github.io/)

## Selected projects

| Project | What it covers |
| --- | --- |
| [Global Economic Prediction](https://github.com/nesaugust/global-economic-prediction-dashboard) | Cleaned and merged country-year indicators, built models for inflation and economic risk, and presented results in Power BI and Streamlit. |
| [Global Tech Insight 2024](https://github.com/nesaugust/Global-Tech-Insight-2024) | Built an R Shiny dashboard to explore compensation, work arrangements and technology preferences in the 2024 Stack Overflow Developer Survey. |
| [Customer Loyalty & Churn Analytics](https://github.com/nesaugust/customer-loyalty-churn-analytics) | Used Power BI, DAX, RFM segmentation and customer lifetime value to identify revenue concentration and retention priorities. |
| [BNPL Credit Risk Dashboard](https://github.com/nesaugust/bnpl-dashboard) | Compared six classifiers for default prediction. XGBoost led on ROC-AUC (0.7824). |
| [Air Quality Prediction](https://github.com/nesaugust/air-quality-prediction-dashboard) | Used hourly pollutant readings and calendar features to estimate PM2.5 with a Random Forest Regressor. |
| [Student Feedback Intelligence](https://github.com/nesaugust/Student-Reviews-Intelligence) | Built a Databricks ETL pipeline with PySpark and Delta tables to prepare Coursera reviews for LLM analysis and Power BI reporting. |
| [NSW Urban Context Benchmark](https://github.com/nesaugust/nsw-urban-context-benchmark) | Led weather data preparation for a team benchmark that tests how LLMs use weather, transport and event context to reason about urban activity. |

## Student Feedback Intelligence

The Databricks pipeline uses three layers:

- **Bronze** ingests Coursera course and review CSVs into Delta tables and deduplicates records.
- **Silver** standardises review text, parses ratings and dates, redacts emails and URLs, separates invalid records, and joins course metadata.
- **Gold** validates theme predictions and checks that quoted excerpts appear in the cleaned reviews. The resulting tables feed Power BI.

GPT-OSS 120B extracts themes, sentiment and supporting excerpts. A TF-IDF and Logistic Regression baseline achieved micro-F1 of 0.6469 and macro-F1 of 0.3824 against LLM-generated theme labels on 99 reviews from held-out courses. These scores measure agreement with the LLM labels.

## Website

The portfolio is a single static `index.html` file with embedded CSS. Open it in a browser to preview changes locally. For a branch-based GitHub Pages setup, commit updates to the branch and folder selected under **Settings → Pages**.
