# Online Shoppers Purchase Intention 2
## A - Data Set

“Online Shoppers Purchasing Intention Dataset” consists of feature vectors belonging to 12,330 sessions.
The dataset was formed so that each session would belong to a different user.<br><br><br>


## B - Attribute Information

**The dataset consists of 10 numerical, 6 categorical and 1 Boolean features. The response variable is also a Boolean variable.**

"Administrative", "Administrative Duration", "Informational", "Informational Duration", "Product Related" and "Product Related Duration" represent the number of different types of pages visited by the visitor in that session and total time spent in each of these page categories. The values of these features are derived from the URL information of the pages visited by the user and updated in real time when a user takes an action, e.g. moving from one page to another<br><br>

**The following three features represent the metrics measured by Google Analytics for each page in the e-commerce site:**

- The value of "Bounce Rate" feature for a web page refers to the percentage of visitors who enter the site from that page and then leave ("bounce") without triggering any other requests to the analytics server during that session.
- The value of "Exit Rate" feature for a specific web page is calculated as for all pageviews to the page, the percentage that were the last in the session.
- The "Page Value" feature represents the average value for a web page that a user visited before completing an e-commerce transaction.

The "Special Day" feature indicates the closeness of the site visiting time to a specific special day (e.g. Mother’s Day, Valentine's Day) in which the sessions are more likely to be finalized with transaction. The value of this attribute is determined by considering the dynamics of e-commerce such as the duration between the order date and delivery date. For example, for Valentina’s day, this value takes a nonzero value between February 2 and February 12, zero before and after this date unless it is close to another special day, and its maximum value of 1 on February 8.

The dataset also includes “Operating System”, “Browser”, “Region”, “Traffic Type”, “Visitor Type” as returning or new visitor. 

There is a Boolean feature called “Weekend” indicating whether the date of the visit is weekend, and month of the year.

The “Revenue” column is a Boolean attribute that used as the class label.<br><br>

The description and link for the data is: http://archive.ics.uci.edu/ml/datasets/Online+Shoppers+Purchasing+Intention+Dataset#<br><br><br>


## C – Initial Model Building with All Features

In the python notebook in this repository, I first build prediction models using all of the features in the data. I use different methods such as:

- Simple Decision Tree Classifier
- Bagged Decision Trees Classifier
- Random Forest Classifier
- Adaptive Boosting Classifier
- Gradient Boosting Classifier
- XGBoost Classifier
- LightGBM Classifier
- CatBoost Classifier<br><br><br>

## D – Feature Selection

I use the “feature_importances_” function to calculate feature importance values. I create much simpler models in which only the most important “n” features are to be found. This way, it is possible to achieve high ROC AUC Scores with much leaner and simpler models.<br><br><br>


## E – Hyperparameter Tuning

I conduct hyperparameter tuning to further improve the ROC AUC Scores of the predictive models.<br><br><br>


## F – Conclusion


