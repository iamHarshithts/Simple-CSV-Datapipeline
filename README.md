# 📊 College Student Placement Data Processing with PySpark

This project demonstrates a complete end-to-end data processing and visualization workflow focused on college student placement analysis. It utilizes **PySpark** for scalable data transformation and **Power BI** for generating interactive visual insights.

## 🚀 Project Overview
The goal of this project is to clean, transform, and analyze a dataset containing student academic, IQ, and placement details. The processed data is then visualized in Power BI to draw insights about factors influencing placements.

## 🧹 Data Processing Pipeline
1. **Data Ingestion**  
   The dataset is loaded using PySpark with automatic schema inference and header detection.
2. **Data Cleaning & Transformation**  
   - **Column Standardization**: Renames columns for better clarity and consistency.
   - **Data Type Fixing**: Converts categorical values like "Yes"/"No" to numeric (1/0) for easier analysis.
   - **Duplicate Detection**: Checks for and flags duplicate records.
   - **Missing Value Check**: Identifies null values across columns.
3. **Feature Engineering**  
   - **Placement Labeling**: Converts binary placement values into human-readable labels like "Placed" or "Not Placed".
   - **Score Aggregation**: Calculates a new feature `Average_Score` based on CGPA, previous semester results, and IQ.
4. **Data Export**  
   After processing, the data is written to a single CSV file, renamed to `FinalCollegeDetails.csv` for clarity and use in Power BI.

## 📈 Power BI Dashboard
The transformed data is visualized through a Power BI dashboard that highlights critical metrics:
- **Placement Overview**  
  A donut chart showing the proportion of placed vs. not placed students, giving an immediate understanding of overall placement success.
- **Average IQ**  
  A KPI card summarizing the average IQ of students, which can indicate general aptitude levels in the student population.
- **Average Score by Placement**  
  A bar chart comparing average scores of placed and non-placed students, useful for performance benchmarking.
- **Top 10 Students by Average Score**  
  A horizontal bar chart showcasing high-performing students with the highest average scores, segmented by placement status.
- **IQ vs Academic Performance**  
  A scatter plot visualizing the relationship between IQ and academic performance, helping to explore potential correlations.

## 💡 Key Insights
- Balanced placement distribution was observed in the dataset.
- Higher average scores were generally associated with placed students.
- No strong linear correlation between IQ and academic performance was evident in the sample shown.

## 📂 Technologies Used
- **PySpark** for data processing and transformation  
- **Python** for automation and scripting  
- **Power BI** for interactive data visualization  

## ✅ Outcome
This project delivers a reproducible workflow that can be used in real-world educational data analytics scenarios. From raw data to clean insights, it offers both technical processing and business-relevant visualization to support decision-making in academic or career support domains.

---

## 👤 Author
iamHarshithts(https://github.com/iamHarshithts)

