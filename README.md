# predicting-next-day-price-direction
Add indicies such as stochastic rsi, moving average, volitility.
instead of one day used to predict the next day, maybe the last 10 days for the next day?


# Random Forest--------------------------------------

## Base Model
window_size = 1000\
step_size = 21\
--- My Model Report ---
              precision    recall  f1-score   support

           0       0.48      0.40      0.44      4004
           1       0.55      0.62      0.58      4623

    accuracy                           0.52      8627
   macro avg       0.51      0.51      0.51      8627
weighted avg       0.51      0.52      0.51      8627

--- Always Up Baseline ---
              precision    recall  f1-score   support

           0       0.00      0.00      0.00      4004
           1       0.54      1.00      0.70      4623

    accuracy                           0.54      8627
   macro avg       0.27      0.50      0.35      8627
weighted avg       0.29      0.54      0.37      8627

## Confident Model
Only confident predictions\
window_size = 1000\
step_size = 21\
--- My Model Report ---
              precision    recall  f1-score   support

           0       0.49      0.28      0.35      1145
           1       0.56      0.76      0.64      1360

    accuracy                           0.54      2505
   macro avg       0.52      0.52      0.50      2505
weighted avg       0.53      0.54      0.51      2505

--- Always Up Baseline ---
              precision    recall  f1-score   support

           0       0.00      0.00      0.00      1145
           1       0.54      1.00      0.70      1360

    accuracy                           0.54      2505
   macro avg       0.27      0.50      0.35      2505
weighted avg       0.29      0.54      0.38      2505

# Logistic Regression--------------------------------

## Base Model
window_size = 1000\
step_size = 21\
--- My Model Report ---
              precision    recall  f1-score   support

           0       0.49      0.37      0.42      4004
           1       0.55      0.66      0.60      4623

    accuracy                           0.53      8627
   macro avg       0.52      0.51      0.51      8627
weighted avg       0.52      0.53      0.52      8627

--- Always Up Baseline ---
              precision    recall  f1-score   support

           0       0.00      0.00      0.00      4004
           1       0.54      1.00      0.70      4623

    accuracy                           0.54      8627
   macro avg       0.27      0.50      0.35      8627
weighted avg       0.29      0.54      0.37      8627

## Confident Model
Only confident predictions\
window_size = 1000\
step_size = 21\
--- My Model Report ---
              precision    recall  f1-score   support

           0       0.50      0.30      0.37      1562
           1       0.54      0.74      0.63      1767

    accuracy                           0.53      3329
   macro avg       0.52      0.52      0.50      3329
weighted avg       0.52      0.53      0.51      3329

--- Always Up Baseline ---
              precision    recall  f1-score   support

           0       0.00      0.00      0.00      1562
           1       0.53      1.00      0.69      1767

    accuracy                           0.53      3329
   macro avg       0.27      0.50      0.35      3329
weighted avg       0.28      0.53      0.37      3329