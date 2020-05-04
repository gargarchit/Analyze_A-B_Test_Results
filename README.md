# Analyze A/B Test Results

Data analysts and data scientists very commonly perform A/B tests. 

Here, I worked to understand the results of an A/B test run by an e-commerce website. The company has developed a new web page to try and increase the number of users who "convert," meaning the number of users who decide to pay for the company's product. My goal was to work through this notebook to help the company understand if they should implement this new page, keep the old page, or perhaps run the experiment longer to make their decision.

## Part I - Probability 

Statistics computed to find out the probabilities of converting regardless of page. These used to analyze if one page or the other led to more conversions.

## Part II - A/B Test 

Next, hypothesis testing was conducted assuming the old page is better unless the new page proves to be better at a Type I error rate of 5%. 

The data were bootstrapped, and sampling distributions were determined for both pages. Conclusions were drawn on conversions for both pages by calculating p-values.

## Part III - Regression

Logistic regression was then performed to confirm the results of the previous steps.  Null and alternative hypotheses associated with this regression model were stated and verified using the statsmodel. 

Next, along with testing if the conversion rate changes for different pages, I added an effect based on which country a user lives. Statistical output using logistic regression was provided to check if the country had an impact on conversion.


## Conclusions 

1) There was no evidence suggesting that those who explore either page lead to more conversions 
2) The country of the user did not impact the rate of conversion between the two pages
