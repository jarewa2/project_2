# Will it rain there?

![Raiin](https://wpcdn.us-east-1.vip.tn-cloud.net/www.myneworleans.com/content/uploads/2021/04/r/y/gettyimages-1257951336.jpg)

## *Table of contents*
* [Project Proposal](#project-proposal)
* [Finding Data](#finding-data)
* [Data Preparation](#data-preparation)
* [Model training & Evaluation](#model-training-and-evaluation)
* [Predictions & Conclusion](#predictions-and-conclusion)

### **Project proposal**

In the interest of the current issues regarding global warming we would like to leverage machine learning algorithms to predict weather patterns and occurences. 

Since we are creating a model that focuses on forecasting weather; we decided to use supervised learning models. A random forest is a bagging-based algorithm that fits a number of classifying decision trees on various sub-samples of the dataset and uses averaging to improve the predictive accuracy and control over-fitting. 
Models used:
- Linear Regression
- Random Forest Regressor
- Random Forest Classifier


### **Finding Data**

We decided to use a static data set from kaggle. The datasets contains 5 years of high temporal resolution (hourly measurements) data of various weather attributes, such as temperature, humidity, air pressure, and weather description for 36 countries.

Static datasets:

[Historical Hourly Weather Data 2012-2017](https://www.kaggle.com/selfishgene/historical-hourly-weather-data?select=wind_direction.csv)


APIs:

[Weather API](https://openweathermap.org/api)



### **Model training & Evaluation**

Linear Regression
- Score of training dataset: 0.1285
- Score of testing dataset: 0.1241
- r2_score of model: 0.1241
- MSE of model: 92.6434
- RSME of model: 9.6251

Random Forest Regressor
- Score of training dataset: 0.929
- Score of testing dataset: 0.4858
- r2_score of model: 0.4858
- MSE of model: 53.5226
- RSME of model: 7.3159


### **Predictions & Conclusion**
We barely scratched the surface! We can leverage more ensemble learners improves accuracy and robustness, as well as decrease variance. Our model showed that precision which was relatively high for predicting both rain and no rain, relates to a low false positive rate. However, there were significant false negatives in predicting rain. The next steps for our project would be to create interactive interface using AWS where users can decide which cities to evaluate/explore.

Additional next steps:
- Create a more robust evaluation to predict other natural occurrences
- Expand current data set to include different countries and cities
- Leverage Weather API



