# SyriaTel-Company-Churn-Analysis
![tel](https://github.com/bvalencia07/SyriaTel-Company-Churn-Analysis/assets/149977850/a188ec14-c084-4b9a-adf2-27e62ffb90ec)
# Overview
This analysis encapsules the search behind determining whether customers for a telecommunication company decide to churn or not by testing various models to see which is most accurate. The said telecommunication company being SyriaTel. All this in hopes of improving their customer retention rates.
# Business and Data Understanding
SyriaTel, the stakeholder, is looking to identify what customers are likely to churn in order to take an active approach to try and retain these customers in order to prevent loss in revenue. By knowing what customers are likely to churn they can identify what aspects of their company need improvement. The word churn refers to how many people choose to stop taking part in a service or product by a company. A [dataset](https://www.kaggle.com/datasets/becksddf/churn-in-telecoms-dataset/data) containing features for customers such as charges, number of calls, and voicemail plans among other things has been provided. To fully understand the data at hand, it will have to be separated between numeric and categorical features as well as put into different predictive models to test which performs best.
# Modeling
### Logistic Regression
![Screenshot 2024-05-20 041545](https://github.com/bvalencia07/SyriaTel-Company-Churn-Analysis/assets/149977850/f1ff3f23-dad2-435d-8267-f5f1bf0379f4)

This confusion matrix indicates that the model correctly predicted 98 instances of a customer churning, and correctly predicted 552 instances where customers didn't churn. However, the model incorrectly predicted 157 instances as not churn as churn. As well as 27 instances that were classified as not churn when they in fact did. The excesive amount of false positives and negatives indicate that this may not be the best model and that it may require some refining.

The logistic regression model seems to have a poor performance. The accuracy, precision, and F1-score all seemed to all be low for both the training and testing dataset.
### Decisioin Tree
![Screenshot 2024-05-20 042504](https://github.com/bvalencia07/SyriaTel-Company-Churn-Analysis/assets/149977850/ec09d07b-3652-42ab-8116-933ce606a595)

This confusion matrix indicates that the model correctly predicted 95 instances of a customer churning, and correctly predicted 650 instances where customers didn't churn. However, the model incorrectly predicted 59 instances as not churn as churn. As well as 30 instances that were classified as not churn when they in fact did. The decision tree seems to be more promising than the logistic regression model, however, there is still overfitting. This could be delt with by either continueing to look into different models or applying hyperparameters.

The decision tree seemed to have a better performance than the logistic regression based on the testing and training scores both being higher on this model than the previous. However, there does seem to be some overfitting as the training data for the precision, recall, and f1 score all seem to be perfect while their testing counterpart is significantly lower in comparison. It is important to note that although some of these scores are higher for this model than the previos, this model still gives the impression it may struggle to properly generalize to unseen data.
### Random Forest
![Screenshot 2024-05-20 042833](https://github.com/bvalencia07/SyriaTel-Company-Churn-Analysis/assets/149977850/6eedd8f9-51eb-4936-9556-83bd0b4fe0e7)

This confusion matrix indicates that the model correctly predicted 100 instances of a customer churning, and correctly predicted 688 instances where customers didn't churn. However, the model incorrectly predicted 21 instances as not churn as churn. As well as 25 instances that were classified as not churn when they in fact did. This being a noticable improvement over the other two models.

The random forest model seems to be even better than the decision tree model. All aspects of the testing model seemed to have quite the improvement with an accuracy going up from 0.89 to 0.94. However, there still seems to be some overfitting due to the training set having a perfect score of 1.0. From here one can either continue to test different models or try to add hyperparameters to fix the overfitting of the model.
### Random Forest with Hyperparameters
![Screenshot 2024-05-20 043056](https://github.com/bvalencia07/SyriaTel-Company-Churn-Analysis/assets/149977850/d84822b1-7dde-4650-a610-bb9020dd3124)

The above revised matrix shows the were 102 instances where the model correctly predicted that a customer would churn and they did, as well as correctly predicting that 690 customers to not churn. However, the model incorrectly predicted 19 instances as not churn as churn. As well as 23 instances that were classified as not churn when they in fact did. None the less, it is an improvement over all the previous models.

The f1-score and the precision went up for the testing data. The recall too had an increase, even though it was a relatively small one. There was a noticable drop in comparison to the previous model in regards to the overfitting.
# Evaluation
![Screenshot 2024-05-20 043421](https://github.com/bvalencia07/SyriaTel-Company-Churn-Analysis/assets/149977850/5ad62f89-5f91-4f44-8a0e-07972f6d4aeb)

This analysis consisted of looking at three basic models being a logistic regression, decision tree, and random forest. After seeing that the random forest performed the best out of the three, hyperparameters were added to them. As shown in the graph above, the four models all have a decent overall performance. Coming in last however is the Logistic Regression curve with an AUC of approximately 0.836. This is followed by the Decision Tree with an AUC of about 0.838. Ultimately leaving the two random forest models with the highest AUC. The original random forest model with an AUC of 0.937 and the Revised with an AUC of 0.934. In this instance, the model that will be chosen will be the Revised Random Forest model due to this model not being overfitted. Even this the other model has a higher AUC, it is a very slim difference of only 0.003.
# Conclusion
Ultimately, the telecommunication company of SyriaTel would be recommended to use the Random Forest model with the applied hyperparameters. The model had an overall accuracy of approximately 94.96%. A further good indicator of a successful model is a high f1-score (0.83), which can only be high if the recall and precision is high. As previously stated, as a company SyriaTel should always look to improve in every way possible for customer improvement, however they should look into the amouont of international calls their customers are making and how much they are charging for international calls. While at it review the voice mail plans that the customers have and customer service.

![tel_2](https://github.com/bvalencia07/SyriaTel-Company-Churn-Analysis/assets/149977850/cbd2feaa-cff8-44aa-b12b-67d194e4551f)


-.gitignore

-README.md

-SyriaTel Churn Analysis.ipynb

-presentation.pdf

-syriatel_churn_data.csv
