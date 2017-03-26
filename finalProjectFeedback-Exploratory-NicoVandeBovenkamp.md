### ***Final Project - Exploratory Analysis Feedback***

***Nico Van de Bovenkamp***
***

**Overall** Fantastic work on the lamda expressions and pulling that data together!

* **Model Tuning:** **Always remember your Train/Test Split**, Regularization, Cross-Validation, Visualizing learning paths, etc.
* **Scaling Data:** Check out the [Standard Scaler](http://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.StandardScaler.html) package. The Standard Scaler will scale all numerical data, which will allow for some easier computation and more efficient computation. This part can actually be quite critical for Regularization.
* * **Feature Importance:** One nice feature of random forests, is the ability to use, and then plot, the `.feature_importance_` of each feature (usually calculated via minimal entropy or gini coefficient). In These types of *why and what factors influence [blank]* problems, the prediction power of a feature can be very handy!
* **Normality of Data** Given the distribution of your data, a non-linear model will likely be your best bet here. That said, a linear model is a smart starting point.
* **Data Transformation** In addition to, or in replace of depending on how everything shakes out, Scaling your data, you should think about doing some data transformations. [Check out this quick guide!](https://www.isixsigma.com/tools-templates/normality/tips-recognizing-and-transforming-non-normal-data/). [This one is also quite good](https://www.isixsigma.com/tools-templates/normality/making-data-normal-using-box-cox-power-transformation/)
* **Model Stacking** Another technique/model architecture that is quite good is to make use of [Stacked Models](https://www.kaggle.com/arthurtok/titanic/introduction-to-ensembling-stacking-in-python). The architecture benefits from the different ways models learn, and aggregates them for better predictions.


***A Table of Key Evaluation Metrics and Visuals:***

*Throwing this in here too! Below is a brief set of many ways you can communicate/measure results that will be useful for your final project. Please let me know if you have any questions!*

| Metrics | |
|--- | --- |
| *Classification* | Accuracy, Precision, Recall, AUC Score, Lift, F-Score, Log-Loss, Gini, Entropy/Information Gain, Statistical Significance (p-value) |
| *Regression* | Mean Squared Error, Mean Absolute Error, Log-Likelihood Estimation, Statistical Significance (p-value) |

| Visualizations | |
|--- | --- |
| *Model Tuning* | Learning Curves, Regularization Learning Paths with an Error Metric, Model Error stepwise increasing feature set size |
| *Classification* | ROC Curve, Feature Importance Charts, Lift Curves, Expected Value Plots |
| *Regression* | Residual plots(!), KDE and KDE of Predicted Values, Expected Value |
