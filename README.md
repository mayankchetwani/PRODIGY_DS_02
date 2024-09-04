# TITANIC DASHBOARD

**Project Overview**
This project was conducted to gain deeper insights into the Titanic disaster by analyzing the demographics of those affected, examining survival rates, and identifying key factors that influenced survival. The goal was to uncover patterns within the data and better understand this tragic event.
![titanic](https://github.com/user-attachments/assets/5195cffa-f531-4093-85ee-1adecce315d8)
**Data Sourcing**
The data used in this project was obtained from publicly available datasets on the Titanic disaster. The dataset includes various details such as passenger IDs, ticket information, survival status, and more. The data was extracted and downloaded in Excel format for further analysis.

**Data Cleaning Process**
The columns containing missing values included Age, Cabin, and Embarked. These gaps were identified for later imputation with appropriate values.

**Feature Types:**
The Titanic dataset contains the following types of features:
- **Categorical/Nominal:** Variables that can be divided into multiple categories without any inherent order or priority. For example, Embarked (C = Cherbourg, Q = Queenstown, S = Southampton).
- **Binary:** A subtype of categorical features with only two possible categories, such as Sex (Male/Female).
- **Ordinal:** Similar to categorical features, but with a clear order or ranking. For example, Pclass (1, 2, 3).
- **Continuous:** Features that can take any value within a specified range, such as Age and Fare.
- **Count:** Features that represent a count of variables, such as SibSp (siblings/spouses aboard) and Parch (parents/children aboard).
- **Useless:** Features that do not significantly contribute to the final outcome of a machine learning model, such as PassengerId, Name, Cabin, and Ticket.
- ![Screenshot 2024-09-04 145900](https://github.com/user-attachments/assets/db614ae7-d508-4181-8212-fe49aec777c1)

After cleaning, the data was uploaded to Power BI for analysis and visualization. The following insights were derived from the data:

**Key Insights:**
- **Sex and Survival:** The survival rate for men was approximately 20%, while for women, it was around 75%. This indicates that gender played a significant role in determining survival chances.
- **Class and Survival:** Passengers in first class had a higher survival rate compared to those in second and third classes, suggesting that Pclass was a strong predictor of survival.
- **Age and Survival:** Children and women aged 20-50 had a higher survival rate, whereas survival decreased for men as age increased. Given the importance of the Age column, missing values should be filled, possibly by using information from the Name column (e.g., titles like Mr., Mrs.) or by applying a regression model. Afterward, an Age_Range column can be created for further analysis.
- **Fare and Survival:** As Fare is a continuous variable, it should be binned (as with Age) to better understand its impact. Higher fares were associated with increased survival rates.
- **Embarked:** The majority of passengers boarded from Southampton (S), so missing Embarked values can be filled with 'S'. Additionally, most third-class passengers boarded from Queenstown (Q), while Southampton seemed favorable for first and second-class passengers compared to third class.

**Conclusion**
Columns like PassengerId, Name, Ticket, and Cabin can be dropped as they are strings, cannot be easily categorized, and do not significantly contribute to the outcome. Columns such as Age and Fare should be converted into range-based columns to retain their predictive power. The Titanic dataset can be further analyzed using additional graph techniques and column correlations. Once exploratory data analysis (EDA) is complete, the refined dataset can be used for predictive modeling.

---

