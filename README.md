# predicting-next-day-price-direction
Add indicies such as stochastic rsi, moving average, etc.
instead of one day used to predict the next day, maybe the last 10 days for the next day?


# Random Forest--------------------------------------

## Base Model
window_size = 1000
step_size = 21
--- Your Model Report ---
              precision    recall  f1-score   support

           0       0.47      0.40      0.43      4096
           1       0.54      0.62      0.58      4730

    accuracy                           0.52      8826
   macro avg       0.51      0.51      0.51      8826
weighted avg       0.51      0.52      0.51      8826

--- Always Up Baseline ---
              precision    recall  f1-score   support

           0       0.00      0.00      0.00      4096
           1       0.54      1.00      0.70      4730

    accuracy                           0.54      8826
   macro avg       0.27      0.50      0.35      8826
weighted avg       0.29      0.54      0.37      8826

## Confident Model
Only confident predictions
window_size = 1000
step_size = 21
--- Your Model Report ---
              precision    recall  f1-score   support

           0       0.49      0.30      0.37      1149
           1       0.58      0.75      0.65      1452

    accuracy                           0.55      2601
   macro avg       0.53      0.53      0.51      2601
weighted avg       0.54      0.55      0.53      2601

--- Always Up Baseline ---
              precision    recall  f1-score   support

           0       0.00      0.00      0.00      1149
           1       0.56      1.00      0.72      1452

    accuracy                           0.56      2601
   macro avg       0.28      0.50      0.36      2601
weighted avg       0.31      0.56      0.40      2601

# Logistic Regression--------------------------------

## Base Model
window_size = 1000
step_size = 21
--- Your Model Report ---
              precision    recall  f1-score   support

           0       0.48      0.37      0.42      4096
           1       0.55      0.66      0.60      4730

    accuracy                           0.52      8826
   macro avg       0.52      0.51      0.51      8826
weighted avg       0.52      0.52      0.51      8826

--- Always Up Baseline ---
              precision    recall  f1-score   support

           0       0.00      0.00      0.00      4096
           1       0.54      1.00      0.70      4730

    accuracy                           0.54      8826
   macro avg       0.27      0.50      0.35      8826
weighted avg       0.29      0.54      0.37      8826

## Confident Model
Only confident predictions
window_size = 1000
step_size = 21
--- Your Model Report ---
              precision    recall  f1-score   support

           0       0.51      0.30      0.38      1551
           1       0.55      0.75      0.63      1779

    accuracy                           0.54      3330
   macro avg       0.53      0.52      0.51      3330
weighted avg       0.53      0.54      0.51      3330

--- Always Up Baseline ---
              precision    recall  f1-score   support

           0       0.00      0.00      0.00      1551
           1       0.53      1.00      0.70      1779

    accuracy                           0.53      3330
   macro avg       0.27      0.50      0.35      3330
weighted avg       0.29      0.53      0.37      3330