# Chronic Disease Prediction

For the purpose of this project, a random forest classifier was utilized to make predictions regarding the presence of chronic kidney disease. The dataset underwent certain preprocessing steps, including the conversion of categorical variables like "rbc" (Red Blood Cell count) into binary values (1 or 0) to represent normal or abnormal, respectively. Moreover, inaccurate values denoted as "\t?" were replaced with NaN, which were then filled with the mean value of the corresponding columns. No duplicate rows were detected in the dataset.

To build a pipeline, Scikit-learn's MinMaxScaler and RandomForestClassifier were employed after dividing the dataset into training and testing sets. 
The algorithm attained an accuracy score of 93%, indicating commendable performance.

To assess the accuracy of the model, a confusion matrix was generated. The classification report derived from the confusion matrix demonstrated that the model performed admirably, exhibiting high precision, recall, and F1-score for both the "with CKD" and "without CKD" classes. This implies that the model effectively differentiated between the two classes.
The high accuracy and consistent performance across various metrics signify the model's reliability for this particular classification task.

Furthermore, the random forest classifier revealed the most influential features in its decision-making process, namely Hemoglobin (hemo), Packed Cell Volume (pcv), Specific Gravity (sg), Red Blood Cell count (rbc), and Albumin (al). 
These selected features hold paramount importance as they reflect essential blood and urine parameters directly associated with kidney function, thereby playing a pivotal role in determining the presence of chronic kidney disease. By considering these significant features, the model is able to make accurate predictions and provide valuable insights into the predominant factors contributing to the classification task.
