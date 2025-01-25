# Summary

## Goal
The goal of the project is to predict whether the price of crypto currency will go up (1) or down (0) 2 weeks from the day of prediction, which is indicated by "Target" column by using the following information:

- ID: ID of each data point (do not include in your model)

- Target: 0 - the price dropped 2 weeks after the time of prediction 1 - the price increased 2 weeks after the time of prediction. This the target variable

- feature_x_y: independent variables from the market data.

- TR_x_EventInd: Event that may or may not affect the crypto currencies price.

- index_1 ~ index_3: the search trend on specific keywords pretaining to crypto currencies.

## Findings

The best model - *Ensemble model* - yielded the following results on the test partition.

1. Weighted F1 score - 0.743

This score suggests that the model is performing reasonably well in terms of both precision and recall across all classes.

2. Recall - 0.724

This indicates that the model is capable of capturing approximately 72.4% of the positive instances, which is a good performance but might be improved further.

3. Precision - 0.799

The model shows that out of all the instances it predicted as positive, around 79.9% are actually positive. This is a good precision score, suggesting the model is quite selective in its predictions.

4. Area under curve - 0.737

This suggests that the model has a moderate level of discrimination capacity. Although, an AUC above 0.7 is considered acceptable, there might be room for improvement.

5. Model's accuracy vs interpretability

Although the ensemble model seems to have achieved a good balance between precision and recall, these scores are lower in comparison to the base model. This indicates some degree of accuracy may be lost in order to gain more interpretability. This could be a characteristic of complex models.

6. Precision vs recall

Finally, precision is slightly higher than recall, indicating that the model may be more conservative in its predictions, preferring to make fewer false positive errors.

## Observations

1. The project explored many ways to treat this dirty dataset - particularly the null values. As there were many null values present when I eyeballed the data, I initially tried to replace all the null values with zero for the purpose of modelling. However, there was some information to be gained from considering imputation as a method. For this reason, I decided to impute null values based on the type of column we were dealing with. For binary column types, I imputed based on the mode of the column. For continuous column types, I imputed based on the mean of the column.

2. Given the size of the dataset being relatively small, I took a  decision to retain as much information as possible. To do this, I avoided dropping any rows or columns and tried to build base models with all information available. I made better progress when we ran a stacking model on top of the predictions from our base models.

3. Among the models I explored, I found that hypertuning and playing with the parameters proved critical to tweaking the F1 score and improving the information gleaned out of each model. Some models worked really well in explaining this dataset such as Random Forest Classifiers and Decision Trees. Interstinglyy, other models such as MLP, Gradient Boosted Trees or SVC models, did not perform as well. The worst performing model I had was the SVC model.

4. Another observation I made was that a single model by itself would not yield a weighted F-1 score higher than 0.719. This was likely due to the fact that the information captured from the complex dataset was limited. My success lay in the fact that I combined results from multiple models using a stacking ensemble which boosted the accuracy of the target class prediction. The only drawback to this approach is the loss of interpretability that is associated with ensemble models.

5. Finally, I also explored strengthening the model by using cross validation and hyperparameter tuning. However, the computational time was quite high. It was an interesting challenge to balance the trade off between interpretability and computational time.
