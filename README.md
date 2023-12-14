# Project Summary/Overview
The overarching goal of our project is to leverage Machine Learning models for predicting and preventing customer churn in banks across France, Germany, and Spain. Success is defined by reducing bank churn, fostering customer retention, boosting satisfaction, and potentially driving revenue growth through retrained customers.
 
In this project, we employed three models, and the random forest model emerged with the highest accuracy during testing. The dataset reflects an overall churn rate of ~20%, signifying a substantial portion of customers at risk. According to the random forest model, the top four factors influencing churn are age, estimated salary, credit score, and balance. Notably, customers activity levels surprisingly ranks among the least impactful factors in predicting churn. This insight guides our strategy towards focusing on key determinants like age and financial metrics to effectively minimize customer churn and enhance overall banking performance.

# Predicting Customer Churn for Bank's Marketing Strategy
Customer Churn is when customers leave the bank entirely. For example, they transfer all deposits to another bank. 56% of customers who left a bank stated their decision could have been reversed. Acquiring new customers is much more costly than retaining an existing one, and most of a bank's revenue comes from existing customers. However, it is now easier than ever to change banks with the growing prevalence of online banking and mobile applications, so effective intervention strategies are imperative for reducing bank churn rates. If it is possible to predict what causes bank churn, it could be possible to target these features within marketing campaigns and promotions to keep existing customers.

# Business Understandng
# Data Understanding
We utilized a bank customer churn dataset from Kaggle, which includes banks in France, Germany, and Spain. We utilized this dataset to help banks predict when a customer would churn to allow for effective intervention and preventative actions to reduce this churn. 


# Modeling and Evaluation
We used three different models: LogisticRegression, DecisionTree, and RandomForest

Using the testing data, we were able to see the accuracy of each model. 

Estimated accuracy of each model:  

Logistic Regression: 0.781  
Decision Tree: 0.774  
Random Forest: 0.840  

As shown by these results, the logistic regression and decision tree models performed roughly the same. 

If we were to just assume every customer did not churn, then the accuracy would be approximately 79.6% (0.796) as this was the percentage of customers who did not churn in the dataset. As shown by the results of the logistic regression and decision tree, these models performed lower than this, making them unviable choices. 

However, the random forest model had an accuracy score of about 84% (0.840). This indicates that the random forest model was able to predict whether a customer would churn or not with a higher degree of accuracy, which makes it the most effective model out of all three. 




# Conclusion
In conclusion, our project aimed at leveraging Machine Learning models to predict and prevent customer churn in banks across France, Germany, and Spain, and has yielded valuable insights. The random forest model, with its high accuracy during testing, identified age, estimated salary, credit score, and balance, as the top factors influencing churn.
 
With an overall churn rate of approximately 20%, signifying a substantial portion of customers at risk, our strategy now focuses on key determinants such as age and financial metrics. Recognizing that customer churn has significant financial implications, our approach aims to minimize churn, foster customer retention, boost satisfaction, and potentially drive revenue growth through retained customers.
 
We emphasize the importance of effective intervention strategies. Given the ease of changing banks in the era of online banking and mobile applications, predictive insights from our model offer a strategic advantage. By targeting influential features identified by the random forest model in marketing campaigns and promotions, banks can enhance overall banking performance and mitigate the costly process of acquiring new customers.

# Repository Navigation
The main branch has all of our final deliverables, including the dataset, readme, and jupyter notebook. The branches in the repo include the
