# Predicting_Nonattandance_by-ML

GoalZone is a fitness club chain in Canada. GoalZone offers a range of fitness classes in two capacities - 25 and 15.
Some classes are always fully booked. However, fully booked classes often have a low attendance rate.
Here our goal was to increase the number of spaces available for classes by predicting whether a member will attend the class or not. When we think that nonattendance is at 70%, predicting nonattendance becomes more important because if we can predict that a member is not going to attend a class, then the number of spaces available could be utilized for other members.

We deployed two models: 1) logistic regression classifier 2) random forest classifier.
When we compare the two models, we can see that the logistic regression classifier has a slightly higher accuracy of 0.774 compared to the random forest classifier's accuracy of 0.747. However, the accuracy is not always the best metric for evaluating a model's performance, especially if the classes are imbalanced (70% nonattendance to 30% attendance here).

Looking at classification reports for the logistic regression and random forest models, we can see that both models performed similarly well in terms of precision for class 0 (non-attendance), with precision scores of 0.78 for the logistic regression model and 0.79 for the random forest model.
Both models also achieved high recall scores for class 0 (the model's ability to correctly identify nonattendance), with recall scores of 0.93 for the logistic regression model and 0.87 for the random forest model.

In terms of F1-score for class 0 (a measure of the overall performance of the classifier, taking into account both precision and recall), the logistic regression model achieved a slightly higher score of 0.85 compared to 0.83 for the random forest model.
Therefore, both models seem to be performing relatively well in identifying individuals who will not attend the fitness class (class 0). However, the logistic regression model performed slightly better in terms of F1-score for class 0. If the main goal is to identify as many nonattendees as possible, then the logistic regression model might be preferred as it has higher recall for nonattendence. However, if the main goal is to make sure that the predicted nonattendees are actually not going to attend, then the random forest model might be preferred as it has higher precision for nonattendance.

It is also important to note here that, the logistic regression model performed better in terms of precision for class 1 (attendance). The random forest model achieved a precision score of 0.63 for class 1, while the logistic regression model achieved a higher precision score of 0.73 for class 1.
The choice of the better model would depend on the specific requirements of the problem. If the main goal is to identify as many attendees as possible, then the random forest regression model might be preferred as it has higher recall for class 1. However, if the main goal is to make sure that the predicted attendees are actually going to attend, then the logistic regression model might be preferred as it has higher precision for class 1.

