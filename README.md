# Capstone Two: Predicting Purchase Likelihood
Springboard repository for Capstone Two projects
## Objective:
This project aims to develop a predictive machine learning model that forecasts the likelihood of individuals making a purchase based on their age, gender, and annual income. This model will assist businesses in optimizing marketing strategies, targeting the right customer segments, and improving overall sales conversion rates.
## Problem Statement:
How can businesses effectively target potential customers to increase purchase rates by understanding the influence of age, gender, and income on purchasing behavior? The challenge is to identify the key demographic factors that drive purchase decisions without overinvesting in ineffective marketing campaigns or neglecting valuable customer segments.

## 1. Data Wrangling
[Data Wrangling Report](https://github.com/celenelouise/Capstone_Two/blob/main/Data%20Wrangling%20Purchase%20Behavior.ipynb)
The data used was acquired from Kaggle and contains information on customer purchase behavior across various attributes. This dataset aims to help understand the factors influencing purchase decisions. The data includes a range of features such as demographic information, purchasing habits, and other relevant characteristics. By analyzing this dataset, I hope to uncover insights and patterns that can inform strategies to enhance customer engagement and increase purchase likelihood.
[Kaggle Dataset](https://www.kaggle.com/datasets/rabieelkharoua/predict-customer-purchase-behavior-dataset)
**Findings:** The dataset was relatively clean, there were no missing or null values, no outliers, and the datatypes all seemed to be appropriate. Although I was able to locate that the dataset included 112 duplicates. These duplicates were all for customers who did not even make a purchase which would significantly skew our data. **Solution:** Removing/dropping these duplicates.

## 2. EDA
[EDA Report](https://github.com/celenelouise/Capstone_Two/blob/main/EDA%20Prediciting%20Purchase%20Behavior.ipynb)
In exploring the data the visualizations made it very clear that there was a distinct relationship between time spent on the site and whether or not a purchase was made. The median time spent with no purchase is around 20 minutes, whereas the median time spent with a purchase is around 35 minutes. 

## 3. Preprocessing & Standardizing 
[Preprocessing Report](https://github.com/celenelouise/Capstone_Two/blob/main/Preprocessing%20and%20Training%20Purchase%20Behavior.ipynb)
Here I found through visualizations that the data had a non-linear relationship between our categorical and numerical features, this helped me make a more informed decision on the type of models that would suit this data best.

## 4. Algorithms & Machine Learning
[ML Report](https://github.com/celenelouise/Capstone_Two/blob/main/Modeling%20Purchase%20Behavior.ipynb)

I chose to use Logistic Regression, Random Forest Classifer, and Gradient Boosting Classifer. Since my correlations are moderate and do not suggest strong linear relationships, ensemble methods like Random Forest and Gradient Boosting made sense. I chose to start with Logistic Regression as it serves as a strong baseline for binary classification and that is exactly what our target variable PurchaseStatus was!

Among the three models, Random Forest is the most suitable choice for this analysis. It delivers superior accuracy (93%) on the test set, consistent cross-validation performance (91%), and interpretability through feature importance analysis. The feature importance provided by Random Forest can help pinpoint the key demographic drivers of purchase decisions—such as annual income, age, or gender—offering actionable insights for businesses to tailor marketing campaigns. For example, focusing discounts or product recommendations on specific age groups or income segments can maximize ROI while minimizing marketing inefficiencies.

## Future Work
Behavioral Features: Integrating behavioral variables, such as website engagement metrics, product categories browsed, or purchase history, to improve model performance.
Advanced Models: Exploring ensemble techniques like stacking or using neural networks for more complex interactions.
Scalability: Validating the models on larger and more diverse datasets to ensure generalizability across various business contexts.
Cost-Benefit Analysis: Applying cost-sensitive learning to optimize for business-specific objectives, such as revenue maximization or customer lifetime value.
