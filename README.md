
# Cat chekr Elimination Classification

Code file has been divided into following sections:
## Sections
1. Importing Libraries
2. Data Preparation
3. EDA 
4. Hypothesis Testing
5. Feature Engineering
6. Modelling

To develop  a Smart Litter System which is equipped with four load sensors capturing any load disturbance happening on the litter box. 
The device functions at 40 Hz frequency rate which means it records 40 samples per second. Multiple devices are used to capture all activities in the 
device in the form of load signals on a day-to-day basis. 

The objective of this project is to develop a solution approach to correctly classify the events as elimination or non-elimination and further classify
the elimination events into urination and defecation.

Using os and glob packages multiple csv and json files are iterated to form a single dataframe.

In sensor data, anomaly data has been observed after the activity is done. As the weights cannot be negative it is considered as wrong entry and 
replaced with zero.

Most of the time domain data and frequency domain features are same and highly correlated so much freq domain features are not taken.

Events with tags such as merged, split, combine, no camera, review and trimmed are removed by detecting the indices thus removing from dataframe.

In section Activity wrt Raw data files are iterated from the folder and raw data from one such folder is visualised

From feature engineering data is divided into 2 models one for classifying between elimination and non elimination and other for urination and 
defecation.

For feature generation Autofeat can be used which generates dependent variables from independent variables but there is no significant improvement in 
model accuracy.

SMOTE analysis is performed on the train data as data is imbalanced.

from logit table depending on p values and heatmap features have been selected

Initial modelling on elimination and non elimination later on urination and defecation is done.





