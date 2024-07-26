# Cognitive-Stress-Level-Prediction-Model

### Project Scope

The scope of this project is to create a stress monitoring system using wearable devices which will examine the Change in blood volume pulse (BVP), heart rate variation (HRV) with the device during stress inducing task. Increased stress is associated with anxiety issues, chronic heart diseases, high blood pressure and nervous breakdown.

This project aims to develop a stress monitoring system with an accuracy of about 80% or higher in predicting stress levels, driven by the possibility of having a real impact on people’s mental health. It focuses on to detect stress at an early stage, which helps in preventing the development of more serious health issues such as abnormal blood pressure or heart diseases. Machine learning models will perform classification of stress levels as 0 for "stress absent" and 1 for "stress present".

### Data Sources

BioStress dataset was used for analysis and model development . The data was collected through 15-minutes long stress inducing session recorded from Empatica E4 device in the presence of a psychologist expert. The collected data is in CSV format. The dataset was converted to one uniform frequency for the ease of analysis for all the physiological signals.

### Tools

- Jupyter Notebook - Exploratory Data Analysis and Model Development
- Amazon Web Services - Storing data (AWS Redshift) and Access Management (IAM Roles)
- PERT Chart - Monitoring the progress
- CRISP DM - Project Development Tool
- Work Breakdown Structure (WBS) - Project Organization Plan
- Gantt Chart - Agile Project Management Tool

### Data Preparation

In the data preparation or cleaning phase, following tasks were performed-

1. Data Loading
2. Handling missing and duplicate values
3. Frequency conversion to 1 Hz for all signals
4. Outlier detection and removal
5. Data Formatting

### Exploratory Data Analysis

EDA was performed on the data and features associated with it-

1. To visualize the frequency distribution of various physiological signals such as Blood Volume Pulse (BVP), Heart Rate Variation (HRV) and Electrodermal Activity (EDA).
2. To understand the statistics of the dataset.
3. To explore relation between features and target variable in the dataset.
4. To handle data imbalance through ADASYN oversampling technique.
5. To perform data standardization for rescaling the features around a mean of 0 and a standard deviation of 1 to prevent impact of outliers.

### Model Development

1. Data is split into test and train sets. 70% of the entire dataset is used for training the model while 15% of the data is kept as test data and 15% of the data is used as validation purpose. This test data is used for model evaluation.
2. Logistic Regression, K-Nearest Neighbor (K-NN), XGBoost Gradient Boosting, Random Forest and Deep Neural Network (DNN) algorithms were implemented to develop machine learning models.
3. Linear, non - linear machine learning techniques and deep learning algorithm were utilized to build robust and accurate models which will perform on unseen dataset effectively.
4. Models were saved as pickle file to avoid the need to retrain it each time we want to run the model.

### Model Architecture

![image](https://github.com/user-attachments/assets/c24df0f7-f9a5-42ef-96a3-8dd3ff676f38)

### Results

1. Logistic Regression, K-Nearest Neighbor (K-NN), XGBoost Gradient Boosting, Random Forest and Deep Neural Network (DNN) performed with an accuracy score of 66%, 92%, 91%, 96% and 92% respectively.
2. Time taken for training the model was recorded and it was observed that Random Forest and DNN took more time to train the models in comparison to others.
3. Receiver Operating Characteristics (ROC) - Area Under the Curve (AUC) values were recorded. Higher value indicates better performance of the model. Random Forest scored highest ROC-AUC value which is 0.99 followed by K-NN (0.96). 

### Future Scope

1. Federated learning can be utilized to address user’s privacy and security concerns. The data used in this project is taken from wearables from the users which might have some sensitive and private information related to the user. Such information should be dealt with care.
2. Along with DNN, other deep learning models can be explored for improved and consistent model’s performance.
