# Amazon_Vine_Analysis


## Overview of the Analysis
In this analysis, an AWS RDS database with tables in pgAdmin was created and datasets from Amazon Review were extracted into DataFrames. Using PySpark, the Amazon book reviews were then analyzed to determine whether having a paid Vine review has any affect on the nuymber of 5-star reviews.

### Results
In this analysis, the amazon reviews were filtered to retrieve all records where the total_votes count was equal to or greater than 20 and then filtered for reviews where the number of helpful votes divided by total votes was greater than or equal to 50%. From the selected reviews, there were a total of 403,807 reviews, of which all reviews were unpaid and there were no paid reviews. 

    * Total Number of Reviews: 403,807
    * Total Number of Paid Reviews: 0 
    * Total Number of Unpaid Reviews: 403,807
          * Total Number of 5-star Unpaid Reviews: 242,889
          * Percentage of 5-star Unpaid Reviews: 60.1%


## Summary
All reviews analyzed for Amazon books were unpaid. There were 403,807 unpaid reviews and zero paid reviews. Of the total unpaid reviews, 60.1% of the reviews were 5-star reviews. It is safe to say there is not any positivity bias in the Vine program for Amazon book reviews, because there were no paid 5-star reviews, and the 5-star reviews received were unpaid and the reviewers had no incentive. To further explore this statement, one could review the other book review datasets available on Amazon.
