# Project Summary/Overview
The overarching goal of our project is to equip banks with our tools to be able to determine customers who would churn and take preventative action through bank products and targeted marketing campaigns based on the results from our binary classification model. We used a dataset with customers from banks in France, Germany and Spain. Success is defined by reducing bank churn, fostering customer retention, boosting satisfaction, and potentially driving revenue growth through customer loyalty as a result of using our model.
 
For the purposes of binary classification, three potential routes were considered: random forest, decision trees, and logistic regression. After having done analysis, logistic regression resulted in being the best fit. The dataset reflects an overall churn rate of ~20%, signifying a substantial portion of customers at risk. According to the logistic regression model, the top four factors influencing churn are age, being an active customer and number of products. This insight guides our strategy towards focusing on key determinants like age and financial metrics to effectively minimize customer churn and enhance overall banking performance.

# Predicting Customer Churn for Bank's Marketing Strategy
Customer churn is when customers leave the bank entirely. For example, they transfer all deposits to another bank. 56% of customers who left a bank stated their decision could have been reversed. Acquiring new customers is much more costly than retaining an existing one, and most of a bank's revenue comes from existing customers. However, it is now easier than ever to change banks with the growing prevalence of online banking and mobile applications, so effective intervention strategies are imperative for reducing bank churn rates. If it is possible to predict what causes bank churn, it could be possible to target these features within marketing campaigns and promotions to keep existing customers.

# Business Understandng
56% of customers who left a bank stated their decision could have been reversed. Acquiring new customers is much more costly than retaining an existing one, and most of a bank's revenue comes from existing customers. However, it is now easier than ever to change banks with the growing prevalence of online banking and mobile applications, so effective intervention strategies are imperative for reducing bank churn rates. If it is possible to predict bank churn it could be possible to target these features within marketing campaigns and promotions to keep existing customers. In order to begin answering this research question, we utilized a bank customer churn dataset from Kaggle, which includes banks in France, Germany, and Spain. We utilized this dataset to help banks predict when a customer would churn to allow for effective intervention and preventative actions to reduce this churn. The ultimate goal of our project and model created is to reduce churn and increase customer retention. With this goal in mind, the benefits include retaining more customers, reducing bank churn rates, and increasing customer satisfaction, all leading to increased revenue due to these lower churn rates. 

# Data Understanding
We utilized a bank customer churn dataset from Kaggle, which includes banks in France, Germany, and Spain. We utilized this dataset to help banks predict when a customer would churn to allow for effective intervention and preventative actions to reduce this churn. 

The dataset contains about 10000 entries. This size ensures that the dataset is large enough to train the model. There are a variety of features in the dataset, such as age, credit score, account balance, and tenure, among others. Churn is represented as a binary value, with 0 referring to a customer that did not churn, and 1 referring to a customer that did. Since units were not specified, we assumed that the currency was USD (US Dollars), and that tenure was in years, not months or days. 

We excluded customers with a balance of zero, as these customers do not produce any profit for the bank. After removing these data points, more features became insignificant, narrowing the focus of the project. The most significant remaining features were age, gender, active member, number of products, and country.

We used a confusion matrix to validate results over a simple accuracy value, as it is better to show the true positives/negatives. We also had to fix the problem of an imbalanced dataset, as there were far more customers who did not churn. This was done using SMOTE, which allowed us to generate synthetic data that would offset this imbalance. After using this technique, there was a reduction in both false negatives and false positives. Overall, true negatives and true positives represented a larger portion of the results. 





# Modeling and Evaluation
We used three different models: LogisticRegression, DecisionTree, and RandomForest

Using the testing data, we were able to see the accuracy of each model. 

Estimated accuracy of each model:  

Logistic Regression: 0.781  
Decision Tree: 0.774  
Random Forest: 0.840  

As shown by these results, the logistic regression and decision tree models performed roughly the same, while random forest had the highest accuracy.

When modelling churn, we knew that we wanted to have a binary classification model to predict the probability of whether or not a customer would churn based on the available features from the dataset. We tested three possibilities: logistic regression, random forest, and decision trees. While Random forest had a higher accuracy than logistic regression, we found that the features that impacted churn were not actionable features for banks to gain insight from and use for marketing campaigns. We decided to use logistic regression, while it had a lower accuracy than random forest, it did reflect features that were significant and impacted churn, the way we had seen in our initial feature analysis. 

Comparing the feature importance and the summary of the logistic regression we found that age and number of products are positively correlated with churn indicating that the probability of churn is likely to increase as age and number of products increases. We also see that being an active member is negatively correlated with churn indicating that if you are an active member there is a lower probability of a  customer churning. We cross-validated these features to find that the relationship of the features with the churn made sense and were reflected in the initial analysis we had done as well. 

While the accuracy is lower, there is more room for generalizability for future data.




# Conclusion
In conclusion, our project aimed at leveraging Machine Learning models to predict and prevent customer churn in banks across France, Germany, and Spain, and has yielded valuable insights. The binary classification model, with its high accuracy during testing, identified age, active member, number of products, as the top factors influencing churn.
 
Recognizing that customer churn has significant financial implications, our approach aims to minimize churn, foster customer retention, boost satisfaction, and potentially drive revenue growth through retained customers.
 
We emphasize the importance of effective intervention strategies. Given the ease of changing banks in the era of online banking and mobile applications, predictive insights from our model offer a strategic advantage. By targeting influential features identified by the binary classification model in marketing campaigns and promotions, banks can enhance overall banking performance and mitigate the costly process of acquiring new customers.

# Repository Navigation
The main branch has all of our final deliverables, including the dataset, this readme file, presentation file and jupyter notebook. The branches in the repo include each member's discoveries as well as analyses. While we have multiple iterations of our jupyter notebook, our final compilation of code is in "FinalCapstoneNotebook.ipnyb". You can find our presentation deck under "Presentation_Pod3" and our dataset under "bank_churn2.csv"
