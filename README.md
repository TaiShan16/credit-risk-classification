# credit-risk-classification
# Credit Risk Analysis Report

### Overview
In this project, we will use various techniques to train and evaluate a model based on loan risk. We use a data set of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of the borrowers. 

We will perform the following step for this supervised learning project:
- Split the Data into Training and Testing Sets
- Create a Logistic Regression Model with the Original Data
- Predict a Logistic Regression Model with Resampled Training Data

### Results
#### Original Data
- The accuracy score on the original data is 99.18% implies that the model's predictions match the true label with a high degree of accuracy, as it correctly predicted approximately 99.18% of the instances in the test dataset.

- Precision measures the proportion of correctly predicted positive instances out of the total instances predicted as positive. It focuses on the accuracy of the positive predictions. In the original data, the "Healthy" loan's precision is 1.00 indicating that all instances predicted as "Healthy" loan are indeed correct. For the "High-Risk" cloan, the precision is 0.85, suggested that 85% of the instances predicted as "High-Risk" are actually correct.

- Recall is the senstivity or true positive rate. It measures the proportion of correctly predicted positive instances out of the total actual positive instances. For the "Healthy" loan, the recall is 0.99, indicating that 99% of the actual "Healthy" loan are correctly identifed. Similarly, for the "High-Risk" loan, the recall is 0.91, suggesting that 91% of the actual "High-Risk" instances are correctly identified.

### Resampled Training Data
- The accuracy score on the resampled training data is 99.38% implies that the model's predictions match the true label with a high degree of accuracy, as it correctly predicted approximately 99.38% of the instances in the test dataset.

- For the "Healthy" loan, the precision is 1.00, which means that all instances predicted as "Healthy" are indeed correct. For the "High-Risk" loan, the prediction is 0.84, indicating that 84% of the instances predicted as "High-Risk" are actually correct.

- For the "Healthy" loan, the recall is 0.99, meaning that 99% of the actual "Healthy" instances are correctly identified. For the "High-Risk" loan, the recall is 0.99, indicating that 99% of the actual "High-Risk" instances are correctly identified.

### Summary
Comparing the two classification reports from original data and resampled data, we observe the following:
1. Precision: 
  - The "Healthy" loan's precision remains the same at 1.00 in both reports, indicating that all instances
    predicted as "Healthy" are correct.
  - For the "High-Risk" loan, the precision is slightly lower in the resampled data (0.84) compared to the 
    original data (0.85). This means that the resampled model correctly predicted a slightly lower proportion 
    of "High-Risk" instances compared to the original model.
    
2. Recall:
  - For the "Healthy" loan, the recall remains the same at 0.99 in both reports, indicating that the models 
    identify nearly all of the actual "Healthy" instances correctly.
  - For the "High-Risk" loan, the recall is higher in the resampled data (0.99) compared to the original data     (0.91). This suggests that the resampled model better captures a higher proportion of the actual 
    "High-Risk" instances.

3. Support:
  - The support values remain the same in both reports, indicating that the number of instances in each type 
    of loan did not change during the resampling process.

Based on the results and comparison of the classification reports, I would recommend using the model for the company because of the following justification:

1. High Accuracy - Both the original data and resampled data models achieved a high accuracy score, high precision and Recall score, which indicating that the model correctly predicts the majority of instances and the model is highly accurate in identifying "Healthy" instances.
2. Class Distribution - If the class distribution in the original data was imbalanced, the use of the RandomOverSampler to address this imbalance can help create a more balanced training data set, which can be beneficial for training a model that new to the data.
