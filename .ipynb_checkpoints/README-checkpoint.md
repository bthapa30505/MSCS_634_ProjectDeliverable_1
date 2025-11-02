
# MSCS_634_ProjectDeliverable_1

# Introduction

For the analysis, I have chosen the dataset related to student performance and various factors that are related to student performance. As a student myself, I am curious to know about the factors that play a major role in academic success. Another reason I chose this dataset is the number of columns it has. It has 20 columns, which are mostly numeric, and will help to perform various calculations to understand the impact of various factors. Additionally, the number of students participating in this study exceeded 5,000, which meets the minimum number of rows required for the dataset to be used for this project.

Also, this dateset contains a diverse set of academic, personal, and socioeconomic factors that influence student performance. With variables like study hours, attendance, parental involvement, motivation level, and family income, it enables the exploration of complex relationships and patterns affecting exam scores. With this dataset, I can apply a variety of data mining techniques such as correlation analysis, classification, regression, and clustering to identify key predictors of academic success. Moreover, the dataset’s mix of numerical and categorical attributes provides opportunities to practice data preprocessing, feature selection, and model evaluation which makes it an ideal, real-world dataset for learning and applying data mining concepts effectively.

Dataset link: https://www.kaggle.com/datasets/anassarfraz13/student-success-factors-and-insights

# Dataset Summary:

Shape: (6607, 20)

1. TOP PREDICTORS OF EXAM SCORE (by correlation):
   2. Attendance: 0.581
   3. Hours_Studied: 0.445
   4. Previous_Scores: 0.175
   5. Tutoring_Sessions: 0.157

2. IMPACT OF CATEGORICAL FEATURES ON EXAM SCORE:
   Parental Involvement:
     - Low: 66.36
     - Medium: 67.10
     - High: 68.09
   Motivation Level:
     - Low: 66.75
     - Medium: 67.33
     - High: 67.70
   Learning Disabilities:
     - No: 67.35
     - Yes: 66.27

3. OUTLIER SUMMARY:
   Features with most outliers:
     - Tutoring_Sessions: 430 outliers (6.5%)
     - Exam_Score: 104 outliers (1.6%)
     - Hours_Studied: 43 outliers (0.7%)
     - Attendance: 0 outliers (0.0%)
     - Sleep_Hours: 0 outliers (0.0%)

# Challenges Faced

Throughout this project,I faced several technical challenges that required careful problem-solving and iterative refinement. One significant obstacle was handling missing values across multiple categorical columns (Teacher_Quality, Parental_Education_Level, and Distance_from_Home), which required implementing appropriate imputation strategies using mode values for categorical data. Another critical challenge emerged during outlier detection and removal, where I faced an IndexingError due to pandas Series index misalignment when creating boolean masks for filtering outlier rows. I was able to resolve this by explicitly setting the Series index to match the DataFrame index using `pd.Series(False, index=df.index)` rather than relying on default integer indexing.
# Conclusion

In conclusion, the exploratory data analysis (EDA) of the student performance dataset provided meaningful insights into the factors influencing academic outcomes. The dataset was found to be well-structured with minimal missing or inconsistent data, ensuring reliable analysis. Key predictors such as Previous Scores, Hours Studied, and Attendance showed strong correlations with Exam Score, highlighting their significance in predicting performance. Additionally, the interactions between categorical and numerical features revealed complex dependencies that could further enhance model accuracy. Overall, these insights serve as a solid foundation for developing robust predictive models aimed at forecasting student exam performance with high precision for the future project deliverables.

