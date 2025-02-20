# Financial-Data-Analysis-Fraud-Detection-in-Microsoft-Fabric-with-PySpark

Project Overview  
This project utilizes Microsoft Fabric Lakehouse for comprehensive financial data analysis, targeting fraud detection, customer segmentation, and transaction trend analysis on a large-scale dataset. The analysis is carried out in PySpark within Microsoft Fabric, leveraging distributed computing for efficient data handling.

Project Workflow  
1. Data Ingestion and Lakehouse Setup:  
   - Created a Lakehouse environment within Microsoft Fabric to manage and analyze the dataset.  
   - The dataset includes transaction records, customer demographics, credit/debit card details, and fraud labels.

2. Data Cleaning and Transformation:  
   - Standardized and cleansed data using PySpark, handling missing values and optimizing data formats.  
   - Generated features like MonthYear and Weekday to enhance trend analysis.  
   - Added an Amount_Type column to distinguish between credit and debit transactions, enabling clearer financial segmentation.

3. Exploratory Data Analysis (EDA):  
   - Conducted extensive analysis on transaction data to uncover patterns and insights:  
     - Transaction Patterns: Aggregated data by MonthYear and Weekday to identify time-based trends.  
     - Fraud Analysis by Merchant ID: Calculated transaction and fraud counts to highlight high-risk vendors.  
     - Geo-Spatial Fraud Trends: Mapped fraud occurrences by ZipCode to identify regional risk patterns.  
     - Year-Over-Year (YOY) Trends: Applied Window functions to calculate YOY transaction changes and identify significant shifts.

4. Fraud Detection Insights:  
   - Focused analysis on fraudulent transactions:  
     - Isolated online transactions without zip codes to examine digital fraud trends.  
     - Identified high-risk segments by analyzing fraud rates by Merchant_ID and ZipCode.

5. Customer Segmentation:  
   - Analyzed customer demographics, including income, age, and credit score, to develop scalable segmentation models and drive personalized insights.

Key Results  
- Fraud Insights: Pinpointed high-risk merchants and regions, providing a data foundation for potential ML-based fraud detection models.  
- Customer Insights: Segmented customer profiles by income and spending, revealing key engagement and risk factors.  
- Transaction Trends: Established clear transaction patterns by month and day, identifying seasonal peaks.

Repository Contents  
- Statistics_Analysis Notebook: Contains the complete PySpark code for data preparation, EDA, trend analysis, and fraud detection, organized into modular sections.

Technical Stack  
- Microsoft Fabric: Lakehouse, Power BI for data warehousing, visualization, and reporting.  
- PySpark: For data engineering, trend analysis, and fraud detection at scale.

Future Work  
1. Develop ML-based fraud detection models, leveraging fraud labels for supervised learning.  
2. Expand geospatial analysis, integrating external datasets for enhanced risk assessment.  
3. Build a real-time monitoring dashboard in Microsoft Fabric and Power BI for proactive alerts.

This repository offers a full-scale pipeline for financial data analysis, fraud insights, and customer analytics, laying the groundwork for further ML and BI applications.
