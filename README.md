# Amazon_Vine_Analysis

## Overview of the analysis: 

Using AWS, SQL, pgAdmin, Colaboratory, Python, and Spark to harness the power of client reviews for marketing data usage.  Are the reviews positive?  Are they negative?  Is there a coorelation between those getting paid and the reviews they leave on products?  With tens of thousands of reviews, on hundreds of thousands of products using ETL and some database 'magic' I can present to the clients what type of data and then analyze it.   I chose to analyze the "Camera" reviews dataset, which also includes some accessories, and cameras from amateur to professional.  

## Results

### Number of Vine Reviews:

![vinenumbs](https://user-images.githubusercontent.com/102183530/180831441-f9f8c806-a914-4eb3-84c2-98198492bc49.png)

-- How many Vine reviews and non-Vine reviews were there? 
  Vine reviews = 607, non-Vine reviews = 50,522.

-- How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
  Vine 5-Star reviews = 257, Non-Vine 5-Star reviews = 25,220.
  
-- What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
  Percentage of Vine 5-Star reviews: 42.34%
  Percentage of Non-Vine 5-Star reviews 49.92%
  
Summary: 
Based on the higher percentage of Non-Vine 5-Star reviews, one could assume there is not bias in the positivity ratings for paid(Vine) vs not paid(non-Vine) reports on Cameras. As always more data would be better at testing and fitting the bias.  I did only analyze items reviewed more than 20 times and deemed "helpful" by over 50% of people reviewing.
I think a good test fit could be a chi-squared, where the star reviews are put into two buckets 1-3, 4-5 with the understanding of a binary "good"/"bad" then able to be converted into a 0/1 module.
A better fit for significance would also be linear regression with the star ratings plotted against vine/non-vine modules and then comparing the p-value and rsquared values.

