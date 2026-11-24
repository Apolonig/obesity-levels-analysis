## Dataset

- **Name:** Obesity Levels
- **Download:** https://www.kaggle.com/datasets/fatemehmehrparvar/obesity-levels
- **Local file:** `data/Obesity_Levels_DataSet.csv`

## Reasons for Choosing the Dataset

1. I am interested in data about people and their everyday habits.
2. I want to learn how to build models for practical prediction tasks.
3. I am interested in applications of machine learning in healthcare.

## Hypotheses

1. A random forest will achieve a higher mean macro F1 score in cross-validation than a single decision tree.
2. A decision tree with its maximum depth selected from a predefined set of values will achieve a higher mean macro F1 score in cross-validation than a tree with no depth limit.
3. Standardizing numerical features will improve the mean macro F1 score of logistic regression compared with the same model without standardization.
4. Adding the interaction feature `FAF × TUE` will improve the mean macro F1 score of logistic regression compared with the same model using only the original features.
5. Removing `CH2O`, `NCP`, and `SCC` will reduce the random forest's mean macro F1 score by no more than 0.01 compared with the model using all features.

## Hypothesis Results

All results below are mean macro F1 scores from the same five stratified cross-validation folds of the training set.

1. **Supported:** The random forest scored **0.9309**, compared with **0.9214** for the single decision tree.
2. **Not supported:** Maximum depths of 15, 20, and 35 matched the unrestricted tree's score of **0.9214**; none of the tested depth limits improved it.
3. **Supported:** Standardization increased logistic regression's score from **0.8140** to **0.8511**, with improvements on all five folds.
4. **Supported in this experiment, with a small gain:** Adding `FAF × TUE` increased the score from **0.8511** to **0.8545**, but improved only three of the five folds.
5. **Supported:** Removing the three features reduced the score from **0.9309** to **0.9286**, a decrease of approximately **0.0023**, below the 0.01 threshold.
