## Student Performance Indicator using Machine Learning

1) Project Overview

  This project predicts student math scores based on various demographic and academic features such as gender, ethnicity, parental education, lunch type, and test preparation. The pipeline includes:

* Data Preprocessing & EDA: Cleaning and analyzing the dataset to identify patterns.

* Feature Engineering: Creating meaningful features to improve model performance.

* Model Training: Applying machine learning models  (e.g., Linear Regression, Decision Trees) to predict math scores.

* Evaluation: Using accuracy, RMSE, and other metrics to assess model quality.

* Deployment: Serving the trained model through a Flask web app, deployed on Microsoft Azure.

2) Dataset:

   Source - [Student Performance in Exams](https://www.kaggle.com/datasets/spscientist/students-performance-in-exams)
   Shape - 1000 rows and 8 columns
   Features - gender, race_ethinicity, parental_level_of_education, lunch, test_preparation_course, math_score, reading_score, writing_score
   Target Variable - math_score

3) EDA (Exploratory Data Analysis)

  Key Insights:

* Gender Distribution: ~50/50 split, but females outperform in reading & writing, while males score slightly higher in math.

<img width="1110" height="543" alt="image" src="https://github.com/user-attachments/assets/6a6779eb-7cc2-4229-9342-bc2a5366f9bb" /></br>


* Ethnicity Impact: Group C and D students perform better on average compared to Groups A & E.

<img width="1113" height="393" alt="image" src="https://github.com/user-attachments/assets/5bfd7ea8-face-4483-b353-55a356b32127" /></br>


* Lunch Effect: Students with standard lunch consistently outperform those with free/reduced lunch across all subjects.

<img width="1108" height="387" alt="image" src="https://github.com/user-attachments/assets/3b03de08-cf01-48e0-b6c5-926ef8c73cb9" /></br>


4) Model Training

Models experimented with:

* Linear Regression
* Decision Tree Regressor
* Random Forest Regressor

Evaluation Metrics:

* Mean Squared Error (MSE)
* Root Mean Squared Error (RMSE)
* R² Score

5) Results

* Random Forest gave the best performance with the lowest RMSE.

* Test preparation and lunch were among the most important predictive features.

* Model generalized well with cross-validation scores aligning closely with training results.

6) Deployment

* Built a Flask web application for predictions.

* Deployed to Microsoft Azure, making it accessible via a web interface.

* Users can input features (gender, parental education, lunch, etc.) and receive a predicted math score.

7) Tech Stack

* Python (pandas, NumPy, scikit-learn, matplotlib, seaborn)

* Flask (backend for serving predictions)

* Microsoft Azure (cloud deployment)

Conclusion:

This project helped me practice the complete machine learning workflow—from cleaning and preprocessing raw data, to performing EDA for insights, to training and evaluating different models. Finally, I deployed the best-performing model with Flask and Azure, gaining end-to-end experience in building and serving ML applications.
 
