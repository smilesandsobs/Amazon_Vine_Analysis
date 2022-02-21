# Amazon_Vine_Analysis

## Overview: The purpose of the analysis of the Vine program.
The Amazon Vine Progam allows manufactures and publishers to pay a small fee to Amazon to have their products reviewed by Amazon Vine members. This includes companies like SellBy who this review is for. We had access to approximatly 50 datasets. I choose to do this anaylysis on the US Video Game dataset. 

Using PySpark we extracted and transformed the dataset to see if there was any bias towards favorable reviews from Amazon Vine members for SellBy stakeholders. 

## Resources:

-Data Souce: [Amazon_Review_Dataset](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt) 
             [us_Video_Games_v1_00.tsv.gz](https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Video_Games_v1_00.tsv.gz) 
              

Software: Python 3.7.12, PYSpark 3.2.1, Google Colab Notebook, PGAdmin 4, Amazon RDS

## Results 

###How many Vine reviews and non-Vine reviews were there?

The dataset included 4,291 paid reviews and 1,781,706 unpaid reviews. 

#### Total Paid Vine Reviews:

![This is an image](https://github.com/smilesandsobs/Amazon_Vine_Analysis/blob/main/total_paid_reviews.png)

#### Total Unpaid Vine Reviews:

![This is an image](https://github.com/smilesandsobs/Amazon_Vine_Analysis/blob/main/total_unpaid_reviews.png)


### How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?

There were 1,607 5 star vine reviews. 


#### Total 5 star vine ratings:

![This is an image](https://github.com/smilesandsobs/Amazon_Vine_Analysis/blob/main/vine_program_star_rating_5.png)
   
### What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

There were a total of 1,026,924 5 star reviews in the dataset. Of those 5 star reviews, 1,025,317 were not Amazon Vine Customers and 1,607 were. 37.5% of the Amazon Vine Customers gave 5 Star Reviews of the video games that they were paid to review. 57.5% of non Amazon Vine Customers gave 5 Star Reviews of a video game. 


## Summary:

While paying Vine customers may help to increase a products number of reviews, it does not guarantee a five star review. In the case of this video game dataset for the US it seems that sufficent customers were reviewing games and a good percentage of them were providing 5 star reviews without any financial motivation. 

One additional analysis which might help support this is to break out the 5 star reviews by game and see which products have more Amazon Vine Reviews and if their reveiews are in general positive. 

