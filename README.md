# Amazon_Vine_Analysis

## Overview

This analysis was conducted to demonstrate the proper methods and processes for working with Big Data. Extensive data on Amazon Kitchen Reviews was accessed through the paid Amazon Vine program, a service that allows manufacturers and publishers to receive reviews for their products.

* In the first portion of this analysis, an ETL was executed using Spark's **High-Level Api:PySpark**  to transform the data, connect to an AWS RDS instance, and load back into pgAdmin. 

* The second portion of this analysis aimed to take a deeper dive into the review data to determine if there is any bias towards reviews that were written as part of the Vine program.  Using **PySpark** we determined if having a paid Vine review makes a difference in the percentage of 5-star reviews.


## Results
Key Results of this analysis are further detailed and pictured below. 

*How many Vine reviews and non-Vine reviews were there?*

* There were a total of 1207 Vine reviews and 97839 non-Vine reviews.

![image](https://user-images.githubusercontent.com/89872154/149710210-eb92c15e-3b14-42ad-959b-45a1a7292c35.png)

*How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?*

* There were 509 Vine reviews with 5 stars and 51,981 non-Vine reviews with 5 stars. 

![image](https://user-images.githubusercontent.com/89872154/149710370-f0db352c-8da7-4519-bf3e-1e058060f29c.png)


*What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?*

* 42.2% of Vine reviews were 5 stars and 53.1% of non-Vine reviews were 5 stars. 

![image](https://user-images.githubusercontent.com/89872154/149710404-e2182991-6021-424b-b9ed-2c9f98ffdc1a.png)


## Summary

This analysis shows that only 509 Vine reviews resulted in 5 star ratings which is farily low considering the 51,981 unpaid reviews that received 5 star ratings. This difference is muted when comparing the percentages of 5 star reviews within the respective paid or unpaid category. To show a statistically significant quantity, trend, or deviation from the norm, we will need to perform additional analysis to calculate the statistical distributeion of paid and unpaid 5 star ratings.
