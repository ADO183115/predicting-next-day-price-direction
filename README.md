# predicting-next-day-price-direction
instead of one day used to predict the next day, maybe the last 10 days for the next day?


# Random Forest--------------------------------------

## Base Model
window_size = 1000\
step_size = 21\
--- My Model Report ---
              precision    recall  f1-score   support

           0       0.48      0.40      0.43      4004
           1       0.54      0.62      0.58      4623

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

           0       0.50      0.28      0.36      1155
           1       0.55      0.76      0.63      1319

    accuracy                           0.53      2474
   macro avg       0.52      0.52      0.50      2474
weighted avg       0.53      0.53      0.51      2474

--- Always Up Baseline ---
              precision    recall  f1-score   support

           0       0.00      0.00      0.00      1155
           1       0.53      1.00      0.70      1319

    accuracy                           0.53      2474
   macro avg       0.27      0.50      0.35      2474
weighted avg       0.28      0.53      0.37      2474

# Logistic Regression--------------------------------

## Base Model
window_size = 1000\
step_size = 21\
--- My Model Report ---
              precision    recall  f1-score   support

           0       0.48      0.38      0.42      4004
           1       0.55      0.65      0.59      4623

    accuracy                           0.52      8627
   macro avg       0.51      0.51      0.51      8627
weighted avg       0.52      0.52      0.51      8627

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

           0       0.49      0.30      0.37      1605
           1       0.55      0.74      0.63      1848

    accuracy                           0.53      3453
   macro avg       0.52      0.52      0.50      3453
weighted avg       0.52      0.53      0.51      3453

--- Always Up Baseline ---
              precision    recall  f1-score   support

           0       0.00      0.00      0.00      1605
           1       0.54      1.00      0.70      1848

    accuracy                           0.54      3453
   macro avg       0.27      0.50      0.35      3453
weighted avg       0.29      0.54      0.37      3453