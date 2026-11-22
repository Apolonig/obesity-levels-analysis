## DataSet
- **Name** - Obesity Levels
- **Link for download** - https://www.kaggle.com/datasets/fatemehmehrparvar/obesity-levels
- **Location dataset** - obesity-levels-analysis/data

## Reasons for сhoosing the Dataset

1. I'm interested in data that pertains to real people
2. I want my model to make predictions that can truly help and be useful
3. I'm interested in the application of machine learning in medicine  

## Hypotheses

1. A random forest will achieve a higher average F1 macro on cross-validation than a single decision tree.
2. A tree with a depth selected from a predefined set of constraints will achieve a higher average F1 macro on cross-validation than a tree without a depth constraint.
3. Standardizing numerical features using StandardScaler will improve the average F1 macro of logistic regression compared to a model without scaling.
4. Adding the FAF × TUE feature will improve the average F1 macro of logistic regression compared to using the original features without this interaction.
5. After excluding CH2O, NCP, and SCC, the average F1 macro score of the random forest will decrease by no more than 0.01 compared to the model using the full feature set.
