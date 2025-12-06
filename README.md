# People-Analytics-Behavioral-Drivers
Behavioral analytics project combining Psychology and Machine Learning. Uses XGBoost & SHAP to decode retention drivers and predict turnover.

Objective:
To enhance employee retention and workplace experience by identifying behavioral, cultural, and organizational drivers of attrition using explainable machine learning.

Overview:
This project reframes the IBM HR Attrition dataset into an employee experience optimization analysis, combining advanced modeling with explainable AI. It leverages XGBoost with class-weight adjustments to address class imbalance, achieving high recall in identifying at-risk employees. Through SHAP explainability, the model reveals which behavioral and workplace factors most influence attrition risk, offering actionable insights for HR strategy, EX design, and leadership development.

Methodology:
•	Data Preparation: Cleaned, encoded, and standardized the dataset after removing redundant columns and duplicates.
•	Modeling: Trained an XGBoost classifier with scale_pos_weight balancing to prioritize recall (early detection of attrition). Logistic Regression was included as a benchmark model.
•	Threshold Optimization: Used precision-recall curve analysis to tune decision thresholds for improved recall on minority (attrition) cases.
•	Explainability: Applied SHAP (SHapley Additive exPlanations) for both global (feature importance) and local (individual employee) interpretability via summary and waterfall plots.

Findings:
•	Optimized model recall improved from 34% → 61%, significantly increasing the model’s ability to identify at-risk employees.
•	Top attrition drivers: Work-life balance, job satisfaction, years since last promotion, and relationship with management.
•	Local SHAP interpretation (waterfall plot) revealed how unique combinations of stressors and satisfaction metrics predicted individual turnover risk.
•	Logistic Regression achieved slightly higher overall accuracy (86%) but lagged in recall, confirming the value of threshold-tuned XGBoost for proactive retention.

Recommendations:
•	Deploy predictive monitoring to flag high-performing but disengaged employees early.
•	Introduce career development pathways and recognition systems for employees at stagnation risk.
•	Use SHAP-based dashboards for real-time EX analytics, enabling HR and management to intervene dynamically.

Impact:
This project demonstrates how behavioral data science can transform HR decision-making — merging psychological insight and machine learning to drive employee well-being, engagement, and retention. The approach directly supports roles in People Analytics, UX Research Analytics, and Behavioral Data Science.

Tools Used:
Python (pandas, XGBoost, SHAP, scikit-learn, matplotlib, seaborn), Precision-Recall Tuning, Logistic Regression Benchmark, IBM HR Attrition Dataset.


