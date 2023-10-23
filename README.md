# King County House Sales Prediction Project

**Author**: [Dominic Muli](mailto:dominic.muli@student.moringaschool.com)

## Project Overview

<img src="./images/syriatel-1.svg" alt="Syriatel" height="100">

Customer churn is a major problem for businesses, especially in the telecommunication industry, where customers can easily switch from one service provider to another. Customer churn refers to the loss of customers who stop using a company’s products or services. A high churn rate can have negative impacts on a company’s revenue, profitability, and growth.

SyriaTel is a company that provides mobile phone and data services. The company was established in 2000 and has its headquarters in Damascus, Syrian Arab Republic.The company wants to reduce its customer churn rate and retain its loyal customers. To do this, the company needs to identify the factors that influence customer churn and predict which customers are likely to leave in the near future.

## Business Problem
The problem statement for predicting customer churn at SyriaTel is as follows:

Given a set of customer data, develop a Python classifier model that can accurately predict which customers are likely to churn.

This model can be used by SyriaTel to identify customers at risk of churning and to implement interventions to prevent them from leaving

## Objectives
* **Develop a Churn Prediction Model**: The primary objective is to create an accurate machine learning model that can predict customer churn at Syriatel based on historical data. This model should provide a reliable indication of which customers are likely to churn in the near future.

* **Identify Key Churn Drivers**: Determine the key factors and customer behaviors that contribute to churn. Understanding why customers leave is crucial for developing effective retention strategies.

* **Implement Proactive Customer Retention**: Utilize the model's predictions to implement proactive customer retention strategies. These strategies should be tailored to the specific needs and risk factors of individual customers.

* **Reduce Churn Rate**: Ultimately, the goal is to reduce the churn rate at SyriaTel. By effectively using the churn prediction model and implementing retention strategies, the company should be able to retain a higher percentage of its customer base.

## Metric of Success
The project will be considered successful if below are achieved:

* **Prediction Accuracy**: The accuracy of the churn prediction model is a fundamental metric of success. This should be measured by assessing the model's ability to correctly classify customers as churners or non-churners. Common evaluation metrics include accuracy, precision, recall, and F1-score.

* **Feature Importance**: Understanding which features or variables are the most influential in predicting churn is crucial. Analyzing feature importance can help SyriaTel focus on the key drivers of customer churn.

* **Reduction in Churn Rate**: The success of the project should be reflected in a measurable reduction in the churn rate compared to the period before the model's implementation. A lower churn rate indicates that the proactive retention strategies are effective.

* **Model Scalability**: If the model proves successful, consider how easily it can be scaled to handle a larger volume of customers and data. Scalability is essential for long-term success.

* **Timely Implementation**: Evaluate how quickly the churn prediction model and associated retention strategies can be implemented to address customer churn issues in a timely manner.

## Understanding Data
The data for this project will be obtained from [Kaggle](https://www.kaggle.com/datasets/becksddf/churn-in-telecoms-dataset).
The dataset has the following variables:

* `state`: The state in which the customer lives.
* `account length`: The number of days the customer has had an account.
* `area code`: The area code of the customer's phone number.
* `phone number`: The customer's phone number.
* `international plan`: Whether or not the customer has an international calling plan.
* `voice mail plan`: Whether or not the customer has a voice mail plan.
* `number vmail messages`: The number of voicemail messages the customer has sent.
* `total day minutes`: The total number of minutes the customer has spent in calls during the day.
* `total day calls`: The total number of calls the customer has made during the day.
* `total day charge`: The total amount of money the customer was charged by the telecom company for calls during the day.
* `total eve minutes`: The total number of minutes the customer has spent in calls during the evening.
* `total eve calls`: The total number of calls the customer has made during the evening.
* `total eve charge`: The total amount of money the customer was charged by the telecom company for calls during the evening.
* `total night minutes`: The total number of minutes the customer has spent in calls during the night.
* `total night calls`: The total number of calls the customer has made during the night.
* `total night charge`: The total amount of money the customer was charged by the telecom company for calls during the night.
* `total intl minutes`: The total number of minutes the customer has spent in international calls.
* `total intl calls`: The total number of international calls the customer has made.
* `total intl charge`: The total amount of money the customer was charged by the telecom company for international calls.
* `customer service calls`: The number of calls the customer has made to customer service.
* `churn`: Whether or not the customer terminated their contract.


## Methods
This project tests a variety of classification models including:

* Decisioin Tree Classifier
* Logistic Regression Classifier
* Random Forest Classifer
* Grid Search CV

## Conclusions
* TThe hyperparameter tuned random forest model is the best model for predicting customer churn, with a high recall of 0.84 for the negative class. However, the model has a lower recall of 0.83 for the positive class, meaning that 17% of actual churners are incorrectly predicted as non-churners.
* It is evident that high customer service calls are the largest contributor to high customer churn.
* Also, it can be observed that the factors including day munites and day charge leading to a higher bill are deterring the customer from continuing their phone plan.
* International plan customers were also seen to switch providers at a higher rate.

### Recommendations
* Focus on reducing the number of customer service calls. This could be done by improving the customer experience, making it easier for customers to find the information they need, and resolving customer issues quickly and efficiently.
* Offer competitive pricing plans and data packages. This could help to reduce churn among customers who are leaving because they are unhappy with their bill.
* Target international plan customers with tailored retention programs. This could include offering discounts, promotions, or other benefits to encourage these customers to stay with the company.

In addition to these general recommendations, the company can also use the insights from the data to develop more targeted retention strategies for specific customer segments. For example, the company could offer customers who have made multiple customer service calls a free month of service or a discount on their next bill. The company could also offer customers who have high day minutes and day charge a data upgrade or a discount on a new phone.

## For More Information

See the full analysis in the [Jupyter Notebook](./customer_churn_prediction_model.ipynb) or review this [presentation](./customer_churn_prediction_model.pdf).

For additional info, contact [Dominic Muli](mailto:dominic.muli@student.moringaschool.com)

## Repository Structure
```
├── data
├── images
├── customer_churn_prediction_model.ipynb
├── customer_churn_prediction_model.pdf
└── README.md
```