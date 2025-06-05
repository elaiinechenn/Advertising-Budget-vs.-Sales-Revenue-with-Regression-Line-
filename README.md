# Advertising Budget vs. Sales Revenue with Regression Line
<img width="736" alt="image" src="https://github.com/user-attachments/assets/baac4b0d-d474-4015-97c1-ff6061b5e9b9" />


<img width="1064" alt="image" src="https://github.com/user-attachments/assets/fcf6aea7-ddd5-4414-a9e8-c86a958b68fb" />

# 
## R² = 0.40（Coefficient of Determination）
🔍 Explanation：
This model can explain 40% of the variation in sales.

In other words, 40% of the changes in sales are driven by the advertising budget. The remaining 60% may be attributed to other factors not included in the model (such as seasonality, distribution channels, promotions, etc.).

✅ A higher R² is generally better, but it’s not the only metric to consider:
R² > 0.7: Often indicates a model with good explanatory power.

A very high R² (close to 1) may also signal overfitting.

## P-value (P>|t|) = 0.000 (for Ad_Budget)
🔍  Explanation：
The p-value tests whether the impact of a variable could simply be due to random chance.

As a general rule, if the p-value is less than 0.05, the variable is considered statistically significant.

✅ In this example:
The p-value for Ad_Budget is 0.000, which is far below 0.05 → This means the advertising budget has a real, statistically significant impact on sales, and it’s not just a coincidence.

## Coefficient (coef) = 2.1419 (for Ad_Budget)
🔍 Explanation：
This means: for every additional 1 unit of advertising budget, sales increase by approximately 2.14 units on average.

This is the most direct metric that can be translated into a business strategy.

✅ Summary：
This model shows that for every additional $1 spent on advertising, sales increase by $2.14 on average. This impact is statistically significant (p-value < 0.05), and the model as a whole explains 40% of the variation in sales (R² = 0.40).

#
## R², P-value, Regression Coefficients Meaning
### 1. R Square（R²，Coefficient of Determination）
R² indicates how well the model explains the variation in the data. Its value ranges from 0 to 1.

Meaning：
R² = 1：The model explains all the variation (ideal).

R² = 0：The model explains none of the variation (like random guessing).

The higher the R², the better the model explains the dependent variable.

Example：
If you're analyzing how ad spending affects sales:

R² = 0.85 means 85% of the changes in sales can be explained by the model (e.g., advertising spend).



### 2. P-value（P 值）
What is it?
The p-value is a statistical metric used to test whether a variable is significantly related to the outcome.

Meaning:
The smaller the p-value, the more statistically meaningful the variable is.


A common threshold is 0.05:

p < 0.05: The variable is statistically significant and likely impacts the result.

p > 0.05: The impact may be due to chance or noise.



Example：
If the p-value for "Facebook Ad Spend" is 0.01, it suggests a statistically significant impact on sales.


### 3. Regression Coefficients（迴歸係數）
What is it？
These represent the influence (or slope) of each variable in the model.

Meaning：
The regression coefficient indicates how much the outcome variable will change for a one-unit change in the independent variable.

The coefficient can be positive (positive impact) or negative (negative impact).

Example：
Suppose your regression formula is:

Sales = 1000 + 2.5 × Ad_Budget

→ This means that for every additional $1 spent on advertising, expected sales increase by $2.50.


# Summary Table
| Name                   | Name in Chinese    | What It Represents             | How to Interpret           |
| ---------------------- | ---- | ---------------- | ------------- |
| R Square (R²)          | 決定係數 | How much variance the model explains        | Higher is better (watch for overfitting) |
| P-value                | P 值  | Whether the variable is statistically meaningful | < 0.05 typically means significant |
| Regression Coefficient | 迴歸係數 | The impact of each variable on the outcome      | Check sign and magnitude     |




