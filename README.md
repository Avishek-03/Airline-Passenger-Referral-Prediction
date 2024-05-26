# Airline-Passenger-Referral-Prediction
The airline industry plays a crucial role in modern transportation, with numerous airlines serving various routes worldwide. To make informed decisions in this highly competitive industry, airlines and stakeholders rely on data-driven insights. Machine learning models are indispensable tools in this regard, allowing for the classification of airlines based on different criteria. This document outlines the development and implementation of an airline classification machine learning model.


This is where machine learning can play a vital role. By using historical customer data, a machine learning model can identify patterns and correlations that indicate a high likelihood of referral. This information can then be used by airlines to target specific customers with personalized marketing campaigns or incentives, increasing the chances of referral and promoting growth.


In conclusion, a machine learning model that predicts the likelihood of referral can provide valuable insights for airlines looking to enhance their customer satisfaction and drive growth through word-of-mouth referrals.

# **Problem Statement**
#### There are few problems that we are looking in this project:

* Develop a classification model to categorize airlines based on the likelihood of customers recommending them to friends and family.

* Recognize the pivotal role of customer satisfaction and referrals in the growth and success of airlines.

* Enable airlines to strategically utilize customer referral information for codeshare agreements, pricing strategies, and market analysis.

* Identify customers likely to refer the airline, a task complicated by the diverse factors influencing satisfaction and referrals.

* Assess the model's capability to provide actionable insights for airlines to tailor services, improve customer satisfaction, and enhance brand reputation.


This problem statement outlines the key objectives, challenges, and considerations for developing a classification model to predict customer referrals in the airline industry.

# **Conclusion**

Our dataset spans from 2006 to 2019, encompassing reviews of various prominent airlines globally. With 131,895 rows and 17 columns, we implemented several data preprocessing techniques to enhance data quality. These included converting date columns to datetime format, refining rating columns, rectifying issues with the "date_flown" column, and managing NaN values appropriately.

During Exploratory Data Analysis (EDA), it was revealed that the economic class was the most popular choice among customers, constituting 72% of bookings, followed by the business class at 19.4%. Ratings were predominantly within the 1-5 range, except for the "overall_rating," which ranged from 1 to 10. Insights gleaned from the EDA process guided subsequent hypothesis testing, wherein t-tests, chi-square, and ANOVA tests were utilized to validate assumptions.

In feature engineering, categorical variables were encoded, and Principal Component Analysis (PCA) was applied for dimensionality reduction. Retaining only the first six principal components, which explained 92% of the data variance, led to a more streamlined dataset with reduced complexity. Subsequently, the data was divided into a training set (70%) and a testing set (30%) for model development and evaluation purposes.

For the classification task, we utilized four models: **Decision Tree, KNN, SVM, and Random Forest**. Initially, the **Decision Tree** model showed signs of overfitting. However, through **cross-validation and hyperparameter tuning**, this issue was addressed effectively. Following this, we proceeded with applying the KNN, SVM, and Random Forest models.

In terms of classification metrics, our business context prioritized F1 score, followed by Precision and Recall, with accuracy ranking third. All four models attained accuracy rates exceeding 90%. After evaluation, SVM emerged as the top-performing model, albeit with a slight advantage.

In the evaluation metrics comparison, SVM demonstrated superior accuracy, establishing it as the preferred choice among the tested models. Remarkably, the most influential features contributing to predictions were identified as "Value for money" and "cabin_service."

The classifier models we developed are essential for predicting passenger referrals, helping airlines identify influential passengers who can boost revenue. Insights from the models emphasize the importance of improving cabin service, ground service, food and beverage offerings, entertainment, and seat comfort to enhance the likelihood of passengers recommending the airline. Prioritizing these key features strategically can drive business growth and elevate customer satisfaction.
