# H1N1-ans-seasonal-vaccines
BUSINESS OVERWIEW

Vaccines provide immunizationfor individuals and enough immunization in a community can further reduce the spread of diseases through 'herd immunity.' In ths project we revisit the public response to previous respiratory diseases i.e the H1N1 influenza virus which had over 150,000 deaths in 2009-2010.

This phone survey asked respondents whether they had received the H1N1 and seasonal flu vaccines, in conjunction with questions about themselves. These additional questions covered their social, economic, and demographic background, opinions on risks of illness and vaccine effectiveness, and behaviors towards mitigating transmission. 

A better understanding of how these characteristics are associated with personal vaccination patterns can provide guidance for future public health efforts through predictive classification modelling

PROBLEM STATEMENT

The government through the National Health Insuarance Fund, prepared a survey to predict wheather people got the H1N1 and seasonal vaccines using information they shared about their backgrounds, opinions and health behaviours. 

We use the data from National Centre of Health Statistics in th United States

The National Health Insuarance Fund would like to usthis information incase of another outbreak to know how to sensitize people more on vaccine practices to be able to enhance the herd immunity and ensuring people live a healthy lifestyle.

OBJECTIVES
1. Use the logistic regression model to predict wheather an individual took the H1N1 vaccine
2. Handle class imbalance in the logistic model to predict wheather one did or did not get the H1N1 vaccine.
3. Use the decision trees model to predict wheather one got the H1N1 vaccine
4. Hyper-parameter tune the dcision trees model to predict wheather one got the H1N1 vaccine
5. Use the logistic regression model to predict wheather an individual took the seasonal vaccine
6. Handle class imbalance in the logistic model to predict wheather one did or did not get the seasonal vaccine.
7. Use the decision trees model to predict wheather one got the seasonal vaccine
8. Hyper-parameter tune the dcision trees model to predict wheather one got the seasonal vaccine


10. This model had an accuracy of almost 85% and can effectively distinguish vaccinated class form unvaccinated class.
The logistic regression model performs better in predicting those who did not get the vaccine with high precision(0.88), recall(0.91) and f1 values(0.90)
For the vaccinated class it has lower precision(0.77), recall(0.70) and f1 score(0.73) thefore less effective in predicting those who actually got the H1N1 vaccine.
![image](https://github.com/user-attachments/assets/83d39335-d9e1-42b2-8bf7-48bca99e5098)

After applying SMOTE, the accuracy dropped from 85% to 83%.
For the unvaccinated class, this tuned model performed better than the original model with high precision(0.92), recall(0.84) and f1 score(0.88) values
For the vaccinated class the tuned model performs poorly with low values for the precision(0.68), recall(0.84) and f1score(0.75) values
![image](https://github.com/user-attachments/assets/9ad68800-8d2a-4c72-9868-a177d4641067)

This decision trees model performed poorly compared to the logistic regression model with lower accuracy of about 76% from 85%.
However, this model performs better in predicting the unvaccinated class with high values for the precision(0.84), recall(0.84) and f1 score(0.84)
As for the vaccinated class, the model performs poorly with low values for the precision(0.62), recall(0.62) anf f1 score(0.62)
After hyperparameter tuning the model, we can see an improvement in the scores but still performs poorly in predicting the vaccinated class.
![image](https://github.com/user-attachments/assets/51b0d480-2406-44cb-a602-1a7ea53754c1)

This model performs relatively well with an accuracy of about 81%
This logistic regression model performs better in detecting the unvaccinated class with high values for precision(0.83), recall()0.84 and f1 score(0.83)
As for the vaccinated class the model performs relatively poorly with lower precision(0.79), recall(0.78) and f1 scores(0.78)
![image](https://github.com/user-attachments/assets/08c7b9d2-91dc-416e-b8a4-8f7648e03c60)

This tuned model achieved an accuracy of  about 81%
The model did not differ so much from the original model with relatively similar values for precision(0.84), recall(0.81) and f1 score(0.83) for the unvaccinated class
For the vaccinated class, there are stll lower values for the precision(0.77), recall(0.80) and f scores(0.79)
![image](https://github.com/user-attachments/assets/c045a989-e835-4e46-9b3a-6ac8279b1607)

This tuned model achieved an accuracy of  about 81%
The model did not differ so much from the original model with relatively similar values for precision(0.84), recall(0.81) and f1 score(0.83) for the unvaccinated class
For the vaccinated class, there are stll lower values for the precision(0.77), recall(0.80) and f scores(0.79)
![image](https://github.com/user-attachments/assets/780976a0-b439-4876-9d6a-a42809ac801d)

This decision trees model achieved an accuracy of about 75%. Performing slightly worse than the logistic regression model.
For the unvaccinated class, there is a drop in precision(0.78), recall(0.75) and f1 scores(0.77) compared to that of the logistic regression model
For the vaccinated class, this model slightly outperforms the logistic regression model with higher precision(0.70), recall(0.73) and f1 score(0.72) values
After tuning the model it outperforms the untuned model with higher values for the metrics in both vaccinated and unvaccinated classes.
![image](https://github.com/user-attachments/assets/c74a5bd9-5f9d-46f3-9ea3-2ae7cddafd62)

### FINAL RECOMENDATIONS
- From the above we can see that all models perform quite well in identifying unvaccinated individuals and relatively poorly in identifying vacccinated individuals.
- The decision tree model performs better than the logistic regression model with higher values for precision and recall.
- After handling the class imbalance in the logistic regression model, there was an improvement in performance if the model with higher precision, recall and f1 values.
- After hyper-parameter tuning the decision trees model, there was also an improvement in the model's performance with higher precision, recall and f1 values
- For the H1N1 vaccine the tuned models outperformed the untuned models improving the predictions for the vaccinated individuals. Although the logistic regression model seems to be performing better than the decision trees models
- For the seasonal vaccines, the untuned logistic regression model, performs poorly in predicting the vaccinated class. After tuning the model it performs slightly better in predicting the vaccinated class. The hyper-parameter tuned decision tree model performs best in predicting both the vaccinated and unvaccinated individuals





