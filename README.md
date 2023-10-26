# Bitcoin-Transaction-Ransomware-Detection

Comparative analysis of hybrid Outlier detection with Machine Learning and Deep Learning Algorithms for Bitcoin Heist Ransomware Detection

The dataset used is from the UCI Machine Learning Repository that contains parsed Bitcoin transaction graphs from 2009 January to 2018 December. The dataset has been curated from three widely adopted studies- Montreal, Princeton and Padua. Using a 24-hour time interval data network transactions have been extracted and the Bitcoin graph is formed. Network edges with less than the threshold minimum of 0.3 bitcoins have been filtered out. This dataset consists of 3000000 observations and 10 attributes to express a specific ransomware transaction pattern. 

The comprehensive data analysis and machine learning pipeline, includes exploratory data analysis (EDA), outlier detection, handling unbalanced data, standardization, and classification. Here's a summary of the key steps and techniques used:

## Exploratory Data Analysis (EDA):

EDA is conducted using correlation heatmaps to visualize the relationships between variables.
Distribution plots (e.g., histograms) and box plots are used to understand the distribution of data and identify potential outliers.
Outlier Detection:

### IQR (Interquartile Range):

The IQR method is applied to detect outliers based on the range between the first quartile (Q1) and the third quartile (Q3). Outliers are identified by values outside the calculated range.

### Isolation Forest:

The Isolation Forest algorithm is used to detect outliers by isolating them from the rest of the data.
It assigns anomaly scores to data points, and those with higher scores are considered outliers.

### DBSCAN (Density-Based Spatial Clustering of Applications with Noise):

DBSCAN is employed for clustering data points based on their density.
Outliers are points that do not belong to any cluster and are identified accordingly.


## Unbalanced Data Handling:

SMOTE (Synthetic Minority Over-sampling Technique) is used to balance the dataset by oversampling the minority class, which can improve classification performance.
Standardization Techniques:

Different data scaling techniques are attempted, including StandardScaler, MinMaxScaler, and RobustScaler, to standardize the features and prepare them for machine learning.

## Classification Algorithms:

Various classification algorithms are used to build models:
- Logistic Regression
- K-Nearest Neighbors (KNN)
- Support Vector Machine (SVM)
- Decision Tree
- Random Forest
- AdaBoost
- XGBoost
- Neural Networks

## Evaluation Metrics:

Model performance is evaluated using standard classification metrics, including:
- Accuracy: Measures the overall correctness of predictions.
- Precision: Measures the percentage of true positive predictions among positive predictions.
- Recall: Measures the percentage of true positives correctly identified.
- F1 Score: A balance between precision and recall, useful for imbalanced datasets.
- ROC (Receiver Operating Characteristic) and AUC (Area Under the Curve): Measure the model's ability to distinguish between classes, particularly useful for binary classification.


