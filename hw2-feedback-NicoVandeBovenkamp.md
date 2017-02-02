### ***Project 2 Feedback***

***Nico Van de Bovenkamp***
***

**Overall:** Great job! And good job making use of statistical tests. That is essential to exploratory analysis, and evaluating assumptions. (Note: my apologies if I went a bit overboard/verbose on my feedback!)

**Some Notes**

* **Q.9:** Great use of statistical tests here! You have interpreted your results very well, and all of the distributions are slightly skewed. However, keep in mind that even if we run a test and it informs us that it is unlikely that the data comes from a normal distribution, we use this information to inform our subsequent models. In other words, if a model is not very working (and it requires assuming normally distributed data) then we may know why. Or, if it is working, we know why it may not be working even better. We will still be building models that are slightly violated by the normality requirement. (Please let me know if this is clear).
* **Q.10:** Again, you are making very key observations here, good work! Keeping in mind my comments on Q.9, you likely won't need to make many shifts given the distribution of the data. Additionally, we don't normally eliminate outliers all-together because remember we are dealing with a sample of the whole population. We aren't entirely confident that those samples are irrelevant to the population. Of course, they are essential to analysis as a whole.
* **Q.12:** Be mindful in your analysis when you make distinctions and definitions. What is a 'smart' student in this analysis? And how does that relate to admission to grad school?
* **Q.13:** You have laid out a very good, concise plan for analysis here! Your plan is pretty much exactly how we will carry out the modeling in the next homework. One important thing to note is the difference between 'classification' and 'regression' problems. We haven't discussed this in class yet, but you would actually be running a Probit model (not an OLS model) for this problem. Both make use of Normal distributions, though Probit is the Inverse CDF function. We will be using a Logit model, but I encourage you to try both!! [Info on Probit vs. Logit models here](https://liberalarts.utexas.edu/prc/_files/cs/Fall2013_Moore_Logistic_Probit_Regression.pdf)
