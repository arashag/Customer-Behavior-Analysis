# Telecom Company Customer Behavior Analysis
A telecom company wants to create a model to recognize the customers that are going to leave the company. At the same time, they want to find the most important factors that contribute to the customers leaving in order to focus and work on them.

The results presentation can be found here: [link](https://github.com/arashag/Telecom-Company-Customer-Behavior-Analysis/blob/master/customer_behavior_analysis.pdf)

## Prerequisites
All the required packages along with their version are in the `requirements.txt`. They can be easily installed with following command:
```
pip3 install -r requirements.txt
```
## Analysis and Result
Because the company's goal is to retain their customers as far as possible, our model needs to have low false negative. In other words, we want to optimize our model to have the highest possible recall score. It turned out that the best recall score is given by random forest classifier (A lot of algorithms have been tested from logistic regression to AdaBoost and CatBoost). The highest recall score is 0.84. Bellow the shap values is used to find the most influencing variables on customer churn:

![shap](https://github.com/arashag/Telecom-Company-Customer-Behavior-Analysis/raw/master/images/shap.png)

Therefore, the most 4 important factors are as follows:
![important factors](https://github.com/arashag/Telecom-Company-Customer-Behavior-Analysis/blob/master/images/customer_behavior_analysis_1_Page_09.png)

Now, we focus on each of them one by one, and provide some recommendations:
![contract type](https://github.com/arashag/Telecom-Company-Customer-Behavior-Analysis/blob/master/images/customer_behavior_analysis_1_Page_10.png)
![internet service](https://github.com/arashag/Telecom-Company-Customer-Behavior-Analysis/blob/master/images/customer_behavior_analysis_1_Page_11.png)
![tenure](https://github.com/arashag/Telecom-Company-Customer-Behavior-Analysis/blob/master/images/customer_behavior_analysis_1_Page_12.png)
![monthly charges](https://github.com/arashag/Telecom-Company-Customer-Behavior-Analysis/blob/master/images/customer_behavior_analysis_1_Page_13.png)
