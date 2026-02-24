# predicting-next-day-price-direction
Add indicies such as stochastic rsi, moving average, etc.
instead of one day used to predict the next day, maybe the last 10 days for the next day?


# Random Forest--------------------------------------

## Base Model
window_size = 1000\
step_size = 21\
--- My Model Report ---

              precision    recall  f1-score   support

           0       0.48      0.40      0.44      4096
           1       0.55      0.62      0.58      4730

    accuracy                           0.52      8826
    macro avg       0.51      0.51      0.51      8826
    weighted avg       0.52      0.52      0.51      8826

--- Always Up Baseline ---

              precision    recall  f1-score   support

           0       0.00      0.00      0.00      4096
           1       0.54      1.00      0.70      4730

    accuracy                           0.54      8826
    macro avg       0.27      0.50      0.35      8826
    weighted avg       0.29      0.54      0.37      8826

## Confident Model
Only confident predictions\
window_size = 1000\
step_size = 21\
--- My Model Report ---

              precision    recall  f1-score   support

           0       0.51      0.30      0.38      1218
           1       0.55      0.75      0.64      1404

    accuracy                           0.54      2622
    macro avg       0.53      0.53      0.51      2622
    weighted avg       0.53      0.54      0.52      2622

--- Always Up Baseline ---

              precision    recall  f1-score   support

           0       0.00      0.00      0.00      1218
           1       0.54      1.00      0.70      1404

    accuracy                           0.54      2622
    macro avg       0.27      0.50      0.35      2622
    weighted avg       0.29      0.54      0.37      2622

# Logistic Regression--------------------------------

## Base Model
window_size = 1000\
step_size = 21\
--- My Model Report ---

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
Only confident predictions\
window_size = 1000\
step_size = 21\
--- My Model Report ---

              precision    recall  f1-score   support

           0       0.51      0.29      0.37      1503
           1       0.55      0.75      0.64      1732

    accuracy                           0.54      3235
    macro avg       0.53      0.52      0.50      3235
    weighted avg       0.53      0.54      0.51      3235

--- Always Up Baseline ---

              precision    recall  f1-score   support

           0       0.00      0.00      0.00      1503
           1       0.54      1.00      0.70      1732

    accuracy                           0.54      3235
    macro avg       0.27      0.50      0.35      3235
    weighted avg       0.29      0.54      0.37      3235