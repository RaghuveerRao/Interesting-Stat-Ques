# Intereseting ML Questions
Loosly built collection of Machine Learning resources 

Q: Specifisit vs Sensitivity  
https://en.wikipedia.org/wiki/Sensitivity_and_specificity

Q: Revise ROC curves and Precision/Recall concepts  
https://developers.google.com/machine-learning/crash-course/classification/roc-and-auc



## Interview Q's
Q: What's the use of AUC  
AUC represents the probability that a random positive (green) example is positioned to the right of a random negative (red) example.  
AUC is desirable for the following two reasons:  
* AUC is scale-invariant. It measures how well predictions are ranked, rather than their absolute values.
* AUC is classification-threshold-invariant. It measures the quality of the model's predictions irrespective of what classification threshold is chosen.

Q: What's the use of Precision - Recall curve

Q: How will you deal with imbalanced dataset techniques  
By designing a cost function that is penalizing wrong classification of the rare class more than wrong classifications of the abundant class, it is possible to design many models that naturally generalize in favour of the rare class. For example, tweaking an SVM to penalize wrong classifications of the rare class by the same ratio that this class is underrepresented.  
https://machinelearningmastery.com/tactics-to-combat-imbalanced-classes-in-your-machine-learning-dataset/  
https://www.kdnuggets.com/2017/06/7-techniques-handle-imbalanced-data.html

Q: What is SMOTE  
SMOTE works by selecting examples that are close in the feature space, drawing a line between the examples in the feature space and drawing a new sample at a point along that line.  
Specifically, a random example from the minority class is first chosen. Then k of the nearest neighbors for that example are found (typically k=5). A randomly selected neighbor is chosen and a synthetic example is created at a randomly selected point between the two examples in feature space. Overall the method suggests first using random undersampling to trim the number of examples in the majority class, then use SMOTE to oversample the minority class to balance the class distribution.  
Borderline-SMOTE: A popular extension to SMOTE involves selecting those instances of the minority class that are misclassified, such as with a k-nearest neighbor classification model. We can then oversample just those difficult instances, providing more resolution only where it may be required.


Q: All else same, in a Random Forest what happens on overfit/underfit scale if I increase the number of trees  
Increasing the number of individual randomized models in an ensemble will never increase the generalization error.
https://datascience.stackexchange.com/questions/1028/do-random-forest-overfit

Q: Bagging/Boosting - Bias/Variance trade of  

Q: What's the difference between LightGBM & XGBoost  

Q: Predict probablistic outpu....  
