# Amazon Vine Analysis - Big Data

## Overview of Project
- Conduct an analysis of Amazon reviews by extracting a dataset into a DataFrame and transform into four seperate tables.
- Use PySpark, Pandas, or SQL to determine if there is any bias toward favorable Vine member reviews in the selected dataset.
- The primary goal is to determine if there is any bias toward favorable reviews from the paid Vine members.
- In this project, we will analyze product data in the Home category.

## Resources
- Software
  - Google Collab Notebook
  - PostgreSQL
  - pgAdmin
  - AWS
- Tools
  - PySpark
  - RDS
- Data Source
  - [Amazon Review Datasets](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt)

## Results

### Extracting the Dataset
Results were extracted from the "More than 20 total votes, More than 50% helpful" table in order to combine reviews with a dataset that provides the best customer rated products with the most helpful votes.
![image](https://user-images.githubusercontent.com/102638461/183811331-78f4c800-1b87-400d-8d44-48627646a199.png)

### Calculating the Totals
Calculations were made in order to determine:
  - Total number of reviews
  - Total paid reviews
  - Total Unpaid reviews
  - Total five-star reviews
  - Total five-star paid reviews
  - Total five-star unpaid reviews
  - Paid & unpaid five star review percentages

![image](https://user-images.githubusercontent.com/102638461/183812983-943f5382-1c7e-4aea-98de-38ebcdc6471e.png)
![image](https://user-images.githubusercontent.com/102638461/183816078-e4935d5c-84ba-4189-9892-a5a63acb979c.png)

In total, there were:
  - 143,285 reviews
  - 2,055 paid reviews
  - 141,230 Unpaid reviews
  - 70,193 five-star reviews
  - 904 five-star paid reviews
  - 71,941 five-star unpaid reviews

And the five star percentages are:
  - 43.99% Vine reviews
  - 50.94% non-Vine reviews

## Summary
Based on the results, there is not enough evidence to prove a strong bias toward five-star reviews from paid Amazon Vine reviewers. 
However this analysis could be further examined by looking all star-rating levels across paid and unpaid reviews. 
Another recommendation for a more thorough analysis should be conducted across multiple different product catagories since some may have greater commerce than one another.


