# Amazon_Vine_Analysis:
The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. We had access to approximately 50 datasets. Each one contains reviews of a specific product, from clothing apparel to wireless products. We picked  one of these datasets, [video game](https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Video_Games_v1_00.tsv.gz). We used PySpark to perform the ETL process to extract the dataset, transformed the data, connected to an AWS RDS instance, and loaded the transformed data into pgAdmin. Next, we used Pandas to determine if there is any bias toward favorable reviews from Vine members in your dataset. We summarized of the analysis for Jennifer to submit to the SellBy stakeholders.



# Resources used:
Data source: Amazon review dataset [click for link](https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Video_Games_v1_00.tsv.gz)
             vinereview dataset [click for link](https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Video_Games_v1_00.tsv.gz)
              Request access for colab [press here](https://colab.research.google.com/drive/1zCawHjfxMX8GqfMJXr8vOLFrQWOYDuxd?usp=sharing)
              
# Results:
-Total Vine number is 94.
-Total 5 stars vine number is 48.
-Percentages of 5 stars reviews is ~51.6%
<img width="839" alt="Screen Shot 2022-02-28 at 9 55 28 PM" src="https://user-images.githubusercontent.com/91306158/156113413-9bd3200b-6f6f-4094-a5ed-06ed1cc18d43.png">

-Total no-Vine number is 40471.
-Total 5 stars non paid vine number is 15663.
-Percentages of 5 stars no-vine reviews is ~38.7%
<img width="840" alt="Screen Shot 2022-02-28 at 9 55 36 PM" src="https://user-images.githubusercontent.com/91306158/156113580-53c64cb1-0529-4253-a3c1-41b825546154.png">

-Total number of vines is 40565
<img width="409" alt="Screen Shot 2022-02-28 at 9 55 43 PM" src="https://user-images.githubusercontent.com/91306158/156113784-940d5b2f-01aa-4f5d-9904-27bf5a25c523.png">


# summary:
We used  Pandas to determine if there is any bias towards reviews that were written as part of the Vine program. For this analysis, we determined if having a paid Vine review makes a difference in the percentage of 5-star reviews.We can see that there is significant difference between vine and no vine reviews which are 51% and 39%, which shows that vine members are bias. We could have more statistical analysis like mean, med, mode to come up with better result.
