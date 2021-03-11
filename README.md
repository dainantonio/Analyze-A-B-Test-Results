# Analyze A/B Test Results
> A/B tests are very commonly performed by data analysts and data scientists. It is important that you get some practice working with the difficulties of these.

> For this project, you will be working to understand the results of an A/B test run by an e-commerce website. The company has developed a new web page in order to try and increase the number of users who "convert," meaning the number of users who decide to pay for the company's product. Your goal is to work through this notebook to help the company understand if they should implement this new page, keep the old page, or perhaps run the experiment longer to make their decision.
> 

Three different approach explored to see whether a new web page would increase the number of users who decide to pay for the product.

Probability approach

12% probability that a user that was in the treatment group converted and the same for the control group. So an almost 50% a user will see the new page

A/B test

It was determined that logistic regression was best for the analysis.
The p-value of determined that we cannot reject the null hypothesis.
a histogram plot of the 10000 values in a numpy array displayed There was no difference in convesion rate, it is centered on zero and symetric.
Regression

Statsmodels was used to fit the logistic regression to see if there is a significant difference in conversion based on which page a customer receives.
Because of the large p-values, we conclude there is weak evidence against null. We therefore retain the null hypothesis.
The hard question is do you stop as soon as one page is considered significantly better than another or does it need to happen consistently for a certain amount of time?

How long do you run to render a decision that neither page is better than another?
