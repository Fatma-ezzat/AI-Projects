## Telecommunication Churn Study
# Made By Fatma Ezzat
### Data Extracted From Kaggle.com

I used colab ,analyze data 
Randomforest model
R^
Regression

R² values range from 0 to 1

1.0 means the feature perfectly predicts the target

0.0 means the feature has no predictive power

Your highest R² = 0.0553 (≈ 5.5%), which is extremely low

Conclusion: No single numeric feature is linearly explaining churn

Even the best feature (OVERAGE) explains only 5.5% of churn variation

Feature	R² Value	Interpretation

~OVERAGE~	0.0553	Weak relationship, but it's the strongest among all numeric features. Customers with more overage minutes may be more likely to churn

~HOUSE~	0.0446	Very weak relationship, but indicates that household size might have a minor impact on churn

~OVER~_15MINS_CALLS_PER_MONTH	0.0409	Very weak, suggests customers making more long calls might churn slightly more

~INCOME~	0.0093	Almost no relationship. Income doesn’t predict churn

~HANDSET_PRICE~	0.0080	Almost no relationship. Handset price has little effect on churn

~LEFTOVER~	0.0037	No meaningful relationship

~AVERAGE_CALL_DURATION~	0.0001	No relationship at all

~All features have very low R² values, meaning no single numeric feature alone can explain churn well

~The highest (OVERAGE at ~0.055) explains only 5.5% of the variance in churn, which is minimal

~This suggests churn is influenced by multiple factors combined, not individually.

~SUMMARY~

~Strong Correlated Features~

~Income~ is strong correlated with ~Handset price~~

~Overage~ is strong correlated with ~over 15min calls per months~~

~Leftover~ is strong negatively correlated with ~Average call duration~~

~Conclusion~ churn depends on interactions between features, not isolated variables

~SUMMARY~

~~Precision (LEAVE = 0.69)~ means that when the customer will leave its correct 69%~

~~Recall (LEAVE = 0.66)~ identifies that 66% of cutomers are actually leaving ~ 34% of churners are missed~ 

~SUMMARY

~Comparing the 2 training models conclude that ~Randon Forest Performance~ is better than ~Logistic Regression Performance~

If ~Probability_Leave~ >= 0.8, ~High Risk~

If ~Probability_Leave~ >= 0.5, ~Medium Risk~

This helps identify customers that might churn even if they didn’t leave yet → actionable insight

