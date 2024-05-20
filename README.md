# SyriaTel-Company-Churn-Analysis
![tel](https://github.com/bvalencia07/SyriaTel-Company-Churn-Analysis/assets/149977850/a188ec14-c084-4b9a-adf2-27e62ffb90ec)
# Overview
This analysis encapsles the search behind determining whether customers for a telecommunication company descide to churn or not by testing various models to see which is most accurate. The said telecommunication company being SyriaTel. All this in hopes of improving their customer retention rates.
# Business and Data Understanding
SyriaTel, the stakeholder, is looking to identify what customers are likely to churn in order to take an active approach to try and retain these customers in order to prevent loss in revenue. By knowing what customers are likely to churn they can identify what aspects of their company need improvement. The word churn refers to how many people choose to stop taking part in a service or product by a company. A [dataset](https://www.kaggle.com/datasets/becksddf/churn-in-telecoms-dataset/data) containing features for customers such as charges, number of calls, and voicemail plans among other things has been provided. To fully understand the data at hand, it will have to be separated between numeric and categorical features as well as put into different predictive models to test which performs best.
# Modeling
### Logistic Regression
![Screenshot 2024-05-20 041545](https://github.com/bvalencia07/SyriaTel-Company-Churn-Analysis/assets/149977850/f1ff3f23-dad2-435d-8267-f5f1bf0379f4)

This confusion matrix indicates that the model correctly predicted 98 instances of a customer churning, and correctly predicted 552 instances where customers didn't churn. However, the model incorrectly predicted 157 instances as not churn as churn. As well as 27 instances that were classified as not churn when they in fact did. The excesive amount of false positives and negatives indicate that this may not be the best model and that it may require some refining.

The logistic regression model seems to have a poor performance. The accuracy, precision, and F1-score all seemed to all be low for both the training and testing dataset.
## Decisioin Tree


## Random Forest


## Random Forest with Hyperparameters


# Evaluation

# Conclusion
