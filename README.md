# Predicting_Online_User_Purchasing_Behaviour
This project adopted Machine Learning models to predict a marketplace's user purchasing intention to reduce churn rate and increase conversion.

### Models Deployed
Logistics Regression, Ensemble Bagging (Random Forest and XGBoost), Deep Learning (Neural Network), Stacking

### Techniques Employed
Exploratory Data Analysis, Resampling Imbalanced Dataset, Feature Engineering, Data Visualization, Machine Learning, Neural Network, Model Stacking

### Tools Employed
SMOTE, sklearn, TensorFlow, Keras, seaborn, plotly

### Context
Over the past decade, online shopping has grown tremendously. Evidently, 46% of total retail sales worldwide comes from e-commerce. However, conversion rate of online shoppers worldwide have been steadily declining, decreasing by 27% from 2018 to 2020. It is thus critical for a marketplace to improve their conversion and retention rate.

Predicting user's purchasing intention will help an e-commerce's operations by preventing churn and increasing purchasing conversion. Furthermore, prediction models can seamlessly integrate with existing operations.

### Datasets
The dataset adopted contained data from a retail site which recorded visitor sessions. Each session represents a different user within 1-year period to avoid user, time and campaign bias. Originally, the dataset contained 12,330 visitor sessions with 10 numerical features and 8 categorical features. <br>

To enrich the dataset, 66 engineered features (including those from one hot key encoding) were created. After feature selection with Recursive Feature Selection (RFE) with Random Forest, the final dataset contained 9 selected features. Through EDA, we found that the dataset was imbalanced, and so, SMOTE was done to resample and balance the data. <br>

### Chosen Model & Performance
Four classification and 1 stacked models were explored to make the prediction: Logistic Regression, Random Forest, XGBoost, Neural Network and Stacked models. The selected performance metrics were ROC-AUC score as it is immune to bias due to size of test data and F1-score as it is robust against imbalanced dataset. Model hyperparameter tuning with Bayes Search CV and Grid Search CV were done to improve performance. <br>

All models have better AUC score when compared to simple OLS, the baseline model. When over-sampling with SMOTE was applied to accommodate for imbalance dataset, all models had better F1 score except for Neural Network model. <br>

The final model which was adopted was Random Forest (with SMOTE) which gave the most balanced score between its F1 and AUC score of 0.68 and 0.917 as compared to other models.
<br>

### Results & Business Impact
Cost-benefit values were derived from the confusion matrix computed from the final model. As compared to the baseline expected revenue, which was based on average industry performance, the classification model will increase revenue by $17.74 per user. <br>

The improvement could be attained from: (a) preventing churn by introducing targeted marketing campaigns and advertisements to high value pages; and (b) from increasing purchasing conversion by improving low value or leaky webpage.

### Collaborators
Georgius Gary Gunawan <br>
Widya Salim <br>
Lam Yan Tung <br>
Susan Koruthu <br>
Patricia Tay
