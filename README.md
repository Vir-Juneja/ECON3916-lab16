# ECON3916-lab16# Regularization: Buying Bias to Sell Variance

## Objective

I explored how LASSO and Ridge regression use regularization to control overfitting and improve predictions compared with OLS when there are many predictors but only a few are relevant.

## Methodology

- I simulated a dataset with 200 predictors, only 5 of which had real effects, and used 105 rows for training.
- I fitted OLS, LASSO, and Ridge regression and compared their test mean squared errors (MSE).
- I traced the LASSO regularization path to see when the true predictors entered the model and when noise variables started appearing.
- I used 5-fold cross-validation to choose the LASSO penalty, fitting the scaler inside each training fold to avoid data leakage.
- I compared LASSO's selected predictors with the known true predictors to count correct selections and false positives.
- I tested how LASSO and Ridge handled two nearly identical predictors by comparing their coefficients.
- I wrote my own AI prompt requesting a cross-validation loop, refined it through [YOUR VALUE] rounds, and compared the AI's selected penalty and CV MSE with my own results.

## Key Findings

- **Test MSE:** OLS had an MSE of [YOUR VALUE], Ridge had [YOUR VALUE], and LASSO had [YOUR VALUE]. This comparison helped me see how regularization affected prediction error.
- **LASSO path:** All 5 true predictors had entered the model by step [YOUR VALUE], while the first noise variable entered at step [YOUR VALUE].
- **Cross-validation:** The selected LASSO penalty was [YOUR VALUE], with a CV MSE of [YOUR VALUE].
- **Variable selection:** LASSO identified [YOUR VALUE] of the 5 true predictors and selected [YOUR VALUE] false positives.
- **Correlated predictors:** When I used two nearly identical predictors, LASSO assigned [YOUR VALUE] to one and zero to the other. Ridge distributed the coefficients as [YOUR VALUE] and [YOUR VALUE].
- **AI comparison:** After [YOUR VALUE] rounds of prompting, I checked the AI-generated cross-validation results against my own implementation. The result was [YOUR RESULT].

Overall, this lab helped me understand the tradeoff between bias and variance, how LASSO performs variable selection, and why scaling and cross-validation matter when choosing a regularization penalty.
