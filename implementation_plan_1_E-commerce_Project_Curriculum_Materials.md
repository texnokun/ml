# Implementation Plan: E-commerce Project Curriculum Materials

This document outlines the technical implementation plan for creating detailed, self-study practical materials (Jupyter Notebooks, datasets, and templates) for the E-commerce project. The materials will strictly follow the 15 topics of the Data Analysis (DA) course and the 15 topics of the Machine Learning (ML) course.

## Goal Description
To generate comprehensive, self-study course materials where students build a single E-commerce analytics project from scratch, passing through all 30 theoretical topics outlined in `data_analysis_plan.md` and `ml_plan.md`.

## User Review Required
> [!IMPORTANT]
> Please review this expanded plan. Is this 30-lesson breakdown exactly what you need, or do you prefer them combined into larger modules (e.g., one notebook covering Pandas 1 & 2)?

## Proposed Changes

### Data Analysis (DA) Course Materials
We will create detailed, self-study notebooks and tasks for each DA topic:

#### [NEW] `da_topic_01_02_intro.md`
- **Topics:** 1. Intro to Data Analysis, 2. Types and sources of data.
- **Content:** Markdown guide on how e-commerce businesses use data. Description of our dataset schema (Customers, Products, Transactions).

#### [NEW] `da_topic_03_04_sheets.md` / `.csv` samples
- **Topics:** 3. Google Sheets 1, 4. Google Sheets 2.
- **Content:** Small CSV exports of our data. Tasks for Google Sheets: building pivot tables for monthly revenue, VLOOKUPs between products and transactions, basic bar charts.

#### [NEW] `da_topic_05_python_intro.ipynb`
- **Topics:** 5. Python Data Analysis.
- **Content:** Self-study guide on Python basics applied to data (lists, dictionaries, loops) using mock customer data.

#### [NEW] `da_topic_06_07_pandas.ipynb` & `_solutions.ipynb`
- **Topics:** 6. Pandas 1, 7. Pandas 2.
- **Content:** Loading the full e-commerce CSVs. Grouping, merging (JOINs equivalent in Pandas), and calculating aggregate metrics (total sales per customer).

#### [NEW] `da_topic_08_data_cleaning.ipynb` & `_solutions.ipynb`
- **Topics:** 8. Data Cleaning.
- **Content:** Handling missing `age` values, removing duplicate transactions, correcting date formats.

#### [NEW] `da_topic_09_10_viz.ipynb` & `_solutions.ipynb`
- **Topics:** 9. Matplotlib, 10. Seaborn.
- **Content:** Visualizing sales trends over time, customer age distribution, and revenue heatmaps by category.

#### [NEW] `da_topic_11_12_13_sql.ipynb` & `_solutions.ipynb`
- **Topics:** 11-13. SQL Basics 1-3.
- **Content:** Connecting to `ecommerce.db` using Python's `sqlite3`. Writing complex `SELECT`, `JOIN`, `GROUP BY`, and window functions to query the database.

#### [NEW] `da_topic_14_statistics.ipynb` & `_solutions.ipynb`
- **Topics:** 14. Basics of Statistics.
- **Content:** A/B testing basics, correlation vs causation, mean/median/mode on the e-commerce transaction data.

#### [NEW] `da_topic_15_da_report.md`
- **Topics:** 15. Report Preparation.
- **Content:** Template and instructions for presenting the EDA findings to a "business stakeholder".

---

### Machine Learning (ML) Course Materials
Following the DA course, students will use their cleaned data to build predictive models.

#### [NEW] `ml_topic_01_02_intro.ipynb`
- **Topics:** 1. ML Overview, 2. Python core topics for ML.
- **Content:** Detailed explanation of supervised vs unsupervised learning in the context of E-commerce (predicting sales vs segmenting users).

#### [NEW] `ml_topic_03_preprocessing.ipynb` & `_solutions.ipynb`
- **Topics:** 3. Data Pre-processing.
- **Content:** Scaling/Normalizing numeric features (price, age), One-Hot Encoding categorical variables (location, gender), Train-Test split.

#### [NEW] `ml_topic_04_05_simple_regression.ipynb` & `_solutions.ipynb`
- **Topics:** 4. Simple Linear Regression, 5. Implementation (Python).
- **Content:** Theory + Scikit-Learn implementation. Predicting a customer's `total_spend` based purely on their `age` or `quantity_of_items`.

#### [NEW] `ml_topic_06_08_multiple_poly_regression.ipynb` & `_solutions.ipynb`
- **Topics:** 6-8. Multiple & Polynomial Regression + Implementation.
- **Content:** Using all available features to predict `total_spend`. Adding polynomial features to capture non-linear relationships.

#### [NEW] `ml_topic_09_11_classification.ipynb` & `_solutions.ipynb`
- **Topics:** 9-11. Classification Theory & Implementation.
- **Content:** Predicting Customer Churn (Binary Classification). Creating a target variable (`churned=1/0`) and training Logistic Regression / Random Forest models. Evaluation metrics (Precision, Recall, ROC-AUC).

#### [NEW] `ml_topic_12_14_clustering.ipynb` & `_solutions.ipynb`
- **Topics:** 12-14. Clustering Theory & Implementation.
- **Content:** Customer Segmentation. Unsupervised learning with K-Means based on RFM (Recency, Frequency, Monetary) scores. Visualizing clusters.

#### [NEW] `ml_topic_15_association.ipynb` & `_solutions.ipynb`
- **Topics:** 15. Association Mining.
- **Content:** Market Basket Analysis. Finding product bundles ("People who buy X also buy Y") using Apriori algorithm.

---

## Verification Plan

### Automated Tests
- Run all python scripts generating notebooks to ensure valid JSON outputs.
- Verify `nbformat` compliance of generated `.ipynb` files.

### Manual Verification
- Manually run all cells in the *Solutions* notebooks locally via Conda/Jupyter to ensure the code executes without errors.
- Verify that the lessons seamlessly bridge the gap between Data Analysis and Machine Learning.
