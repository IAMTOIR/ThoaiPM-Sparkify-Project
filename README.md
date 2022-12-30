# **Sparkify - Churned Users Project**


## **Table of contents**

- [Project Descriptions](#project-descriptions)
- [Blog post](#blog-post)
- [Project Steps](#project-steps)
- [Improvements](#improvements)


## **Project Descriptions**

Sparkify is an imaginary start-up that offers a music streaming service to users in the United States. Customers can choose between a free tier with advertisements or a premium subscription with a flat monthly fee. The service allows users to change, upgrade, or cancel their subscriptions at any time. It is important for Sparkify to keep its users satisfied because every time a user interacts with the service, it generates data that can provide insights on how to improve the service and keep the business thriving. To predict which users are likely to churn (downgrade to the free tier or cancel their subscription entirely), the data team analyzes log files that contain information about each user interaction, such as the user's ID, the name of the song played, the length of the song, and the artist's name. However, the log file has become too large to be processed on a standard desktop computer, so Sparkify has turned to the Apache Spark distributed file system. Udacity provides a 12GB dataset on AWS S3 that can be used to analyze the data using a Spark cluster on the cloud through AWS or IBM Cloud.

## **Blog post**
You can find a brief blog entry I wrote on Medium: https://medium.com/@pmthoai2304/sparkify-churned-user-project-6fca93854014
This is the GitHub link to my project: https://github.com/IAMTOIR/thoaipm-DS_capstoe

## **Project Steps**
- Load data into Spark
- Explore and Clean Data
- Create Features
- Build Models
- Predict Churn

In this project, we examine a tiny portion of the user data on Sparkify's Log file using Spark SQL and Spark Dataframes. To forecast user churn at Sparkify, we make use of the Machine Learning Library (MLlib) in PySpark. We find some features in the user data that can aid in the detection of impending churn after reviewing the subset of the Log file. To train ML models, we compile a collection of characteristics for each user in the subset. We next assess how well four MLlib classification models do at predicting churn (Logistic regression, Random Forest classifier, Gradient-boosted tree classifier, Linear Support Vector Machine).

After evaluating the models, we determine that the random forest classifier is the best performer. Since the number of churned users is relatively small, we use the F1 score as the metric to optimize. To maximize the use of available data and gain more insight into the algorithm's performance, we employ cross-validation.

## **Improvements**
There are several ways to potentially improve the current results:
- Increasing the dataset size by using the full 12GB dataset
- Experimenting with different parameters for the selected models
- Adding additional features, such as customer location (city/state), which may be relevant for predicting churn. For example, some states may have higher churn rates due to certain lifestyle factors or the nature of the environment, while others may have lower churn rates due to a more settled and resistant to change population.


