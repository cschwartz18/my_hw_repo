### ***Project 3 Feedback***

***Nico Van de Bovenkamp***
***

**Overall:** Good work on this homework! You made great use of several packages, and exhibit that you have a solid understanding of what odd rations and how logistic regression works. And nice work on the odds ratios!!

**A note on modeling:**
At times, model evaluation and evaluation metrics can get a bit lost because we spend a lot of time just understanding what these models are and how to run them. Think about what metrics you could use to measure how well your model learned the data! ROC Curves and AUC scores are very, very handy for classifiers. And try out some different models, hyper-parameters (regularization), cross validation, and loss-functions.

* **Q.4.4** Note that when calculating those confidence intervals, we usually want to find the confidence interval of the Odds Ration. What you had calculated is the confidence interval for the Log Odds Ration. Thus:
```python
#Get Conf interval
conf_interval = result.conf_int()
#Get log odds ratios
log_odds_ratio = result.params
# Append the actual log odds ratios to confidence interval
conf_interval['Odds Ratios'] = log_odds_ratio
# Rename columns
conf_interval.columns = ['2.5%','97.5%','Odds Ratios']
# Print the Odds Ratios (Not the Log Odds!)
print(np.exp(conf_interval)
```
