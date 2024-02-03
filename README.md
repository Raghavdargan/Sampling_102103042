# TITLE : Exploring Sampling Methods and Applying different Models
By Raghav Dargan 102103042 

# 1. Methodology
![image](https://github.com/Raghavdargan/Sampling_102103042/blob/main/methadology_sampling.png)

# 2. Description
## Stage 1:
In this Assignment, We were given a Credit Card Dataset comprising of 772 instances and 31 features, out of whixh on checking it was found that the data had 763 instance of Class 0 and only 9 instances of Class 1, pointing to the fact that the dataset is highly imbalanced.

In order to balance the dataset => normalise function is being used

## Stage 2:
Now 5 different Sampling Techniques were applied on the Balanced Dataset ,which are mentioned as below :

(i) Simple Random Sampling:
Randomly selects a specified number of samples from the dataset without any specific criteria.

(ii)Stratified Sampling:
Divides the dataset into strata or groups based on a specific feature (e.g., class labels).

(iii)Cluster Sampling:
Divides the dataset into clusters or groups.
Randomly selects entire clusters and includes all samples within those clusters in the sample.

(iv)Bootstrap Sampling:
Creates multiple samples by randomly resampling with replacement from the original dataset.
Useful for estimating the distribution of a statistic or creating multiple datasets for model training.

(v)Systematic Sampling:
Selects samples at regular intervals after an initial random start.
Requires defining a sampling interval, and it's less prone to bias than simple random sampling.

## Stage 3:
After applying the Sampling techniques on the Balanced Dataset, each of the samples were splitted into train and test data and fed into 5 different models and an Accuracy Score was obtained.

Following are the Models that were used :

(i)Logistic Regression:
A binary classification algorithm that models the probability of a binary outcome.
It's interpretable and provides coefficients for each feature, indicating their impact on the outcome.

(ii)Decision Tree:
A tree-like model where each node represents a feature, each branch a decision, and each leaf an outcome.
It's capable of handling both classification and regression tasks and is interpretable.

(iii)XGBoost:
XGBoost is an ensemble learning algorithm that uses a gradient boosting framework, excelling in both speed and performance for classification and regression tasks.

(iv)SGD Classifier:
 Stochastic Gradient Descent (SGD) Classifier is a linear classifier optimized using stochastic gradient descent, suitable for large-scale machine learning problems due to its efficiency and ease of implementation.

(v)Extra Tree:
Extra Trees, or Extremely Randomized Trees, is an ensemble learning method that builds multiple decision trees and combines them to improve accuracy, robustness, and control overfitting in classification and regression tasks.

# 3. Output
Subsequent to the creation of five distinct samples utilizing these techniques, each sample underwent evaluation using five different models. The accuracies of each model for a given sample are summarized in the following table:

|Sampling Techniques|Logistic Regression|XGBoost|SGD Classifier|Extra Tree|Decision Trees|
|-------------------------|---------------|---------------------|--------|----------------|----------|
| Simple Random Sampling   | 0.8571        | 0.9740             |  0.8312|  0.9870         | 0.9610  |
| Systematic Sampling      |  0.8859     | 1.0000           | 0.7651 |  0.9866         | 0.9933   |
| Cluster Sampling         | 0.9605      | 1.0000              |0.9605 | 1.0000         |  1.0000   |
| Stratified Sampling      | 0.8881        | 0.9851              | 0.9254 |  0.9552         | 0.9851   |
| Bootstrap Sampling       | 0.9250        | 0.9500              | 0.9500 | 0.9875         | 0.9750   |


 # 4.Result 

From the table conclusion can be drawn that Decission Trees is best model and if we consider 1 as overfitting then XG will be the best

 
