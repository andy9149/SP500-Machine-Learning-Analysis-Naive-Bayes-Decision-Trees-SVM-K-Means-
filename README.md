# SP500-Machine-Learning-Analysis-Naive-Bayes-Decision-Trees-SVM-K-Means-
Machine learning analysis predicting and classifying 26,000+ companies by financial indicators (2000–2024). Implements Naïve Bayes, Decision Trees, SVM, and K-Means Clustering to forecast P/E ratios and segment industries.

💹 Financial Markets Prediction & Classification

Author: Sebastian Heredia
Course: BSAN6070 – Introduction to Machine Learning
Tools: Python (Scikit-learn, Pandas, NumPy, Matplotlib, Seaborn)

📘 Overview

This project applies machine-learning algorithms—Naïve Bayes, Decision Trees, Support Vector Machines, and Clustering—to analyze and predict financial market behavior.
Using data from 26,000+ companies (2000 – 2024), the goal is to classify firms by industry group and predict Price-to-Earnings (P/E) ratios based on key financial indicators such as EPS, Working Capital, Book Value, Debt, and Capital Expenditure

Lab3-5 Financial Markets Predic…

.

🧩 Project Files
File	Description
Lab3.ipynb	Data cleaning, descriptive analytics, winsorization, and correlation analysis

LAB 3 DESCRIPTIVE ANALYTICS Win…

.
Lab4.ipynb	K-Means clustering analysis on Winsorized CapEx and Long-Term Debt

LAB 4 CLUSTERING

.
Lab5_Decision Trees.ipynb	Decision-Tree classifier with financial features (10 predictors, 27 industries)

LAB 5 DECISION TREE

.
Lab5_KNN.ipynb	K-Means & KNN clustering and visualization

LAB 5 CLUSTERING KNN

.
Lab5_NB.ipynb	Naïve Bayes classifier for multi-class industry prediction

LAB 5 NAÏVE BAYES

.
Lab5_SVM.ipynb	SVM regression & classification models with GridSearchCV hyperparameter tuning

LAB 5 SVM

.
Lab3-5 Financial Markets Prediction Classification.pdf	Final report summarizing methodology, analysis, and results

Lab3-5 Financial Markets Predic…

.
⚙️ Methodology
1️⃣ Data Preprocessing

Dataset reduced to fiscal years 2000–2024 (235 996 records × 301 features).

Removed columns with > 50 % missing values.

Median imputation for numerical NAs; irrelevant categorical fields dropped.

Outliers handled via winsorization (1st–99th percentiles); all numeric fields log-transformed.

2️⃣ Descriptive Analytics

Correlation Matrix: EPS and Net Income strongly positive (~0.9).

EPS by Year: Post-2010 stability and growth; dips in 2008 & 2020 reflect crisis periods.

Boxplots & Scatterplots: EPS vs NI show positive correlation and high dispersion

LAB 3 DESCRIPTIVE ANALYTICS Win…

.

3️⃣ Classification Models
Model	Accuracy	Key Findings
Naïve Bayes	17.6 %	Poor performance; feature independence assumption invalid

LAB 5 NAÏVE BAYES

.
Decision Tree	39.8 %	Better results; max_depth = 5 balances fit and generalization

LAB 5 DECISION TREE

.
SVM (Linear)	85 %	Best accuracy & F1 ≈ 0.84; handles high-dimensional data effectively

Lab3-5 Financial Markets Predic…

.
4️⃣ Clustering Analysis

K-Means (k = 8) identified distinct industry segments with P/E ratio and EPS patterns.

Hierarchical Clustering: Silhouette score 0.46 with 4 clusters revealing financial strength tiers

LAB 5 HIERARCHICAL CLUSTERING

.

📊 Key Insights
Insight	Interpretation
SVM dominates	Linear kernel (C = 10) yielded 85 % accuracy and balanced precision/recall

LAB 5 SVM

.
Decision Tree bias	Overfits to dominant classes with weak recall for minor industries

LAB 5 DECISION TREE

.
Naïve Bayes fails	Independence assumption breaks for correlated financial metrics

LAB 5 NAÏVE BAYES

.
K-Means segmentation	Revealed growth vs risk clusters useful for investment screening

LAB 5 CLUSTERING KNN

LAB 5 HIERARCHICAL CLUSTERING

.
💡 Business Application

Investor Targeting: Identify undervalued or high-growth firms by cluster profile.

Risk Assessment: Distinguish financially weak vs strong companies for credit or M&A.

Benchmarking: SVM industry classification enables peer comparison and sector forecasting.

🚀 Future Work

Introduce financial ratios (e.g., ROA, Debt/Equity) to improve class separation.

Explore ensemble methods (Random Forest, XGBoost) and deep learning architectures.

Integrate textual sentiment data from filings or news for multi-modal prediction

Lab3-5 Financial Markets Predic…

.

📬 Contact

Sebastian Heredia
📧 andy_9149@hotmail.com
🔗 [LinkedIn](https://www.linkedin.com/in/seb-heredia/)  
💻 [GitHub](https://github.com/andy9149)
