# Amazon_Vine_Analysis

## Project Overview
**Purpose**: The purpose of this project was to create flexible code that can quickly perform ETL on Amazon reviews datasets and analyze how helpful Amazon's paid "Vine" reviews are for these products. To accomplish this I performed the follwing:

1. Used Amazon Webservices to create a relational database instance (PostgreSQL)
2. Used pgAdmin to create tables to store the Amazon Review Data
3. Used GoogleColab to create a PySpark Session and Performed ETL on the datasets
4. Used GoogleColab and PySpark to determine if Vine reviews (paid) are helpful to consumers relative to unpaid reviews

## Resources
**Amazon Review Datasets**

https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt

**PySpark ETL Code**

[ETL Code](Amazon_Reviews_ETL.ipynb)

**Vine Analysis Code**


[Musical Instruments](Vine_Review_Analysis_Instruments.ipynb)

[Digital Video Games](Vine_Review_Analysis_DigVideoGames.ipynb)

## Results
**Analysis Overview**: The key objective of the analysis was to compare paid vs unpaid reviews. I originally chose to analyze datasets from Digital Videogames, however, this dataset did not contain any paid reviews. So, instead I analyzed reviews for Muiscal Instruments. 

In order to compare paid and unpaid reviews I only analyzed reviews that had a high number of votes (<=20). I then filtered the dataframes so that the ratio of helpful votes to total votes was at least 50%. I then filtered the dataframe based on reviews from the paid service (Vine == "Y") or unpaid (Vine == "N") and compared the total number of reviews, the number of 5-star reviews, and the percentage of 5-star reviews in each category.

**Results for Paid Reviews for Musical Instruments**

Total Number of Reviews = 

Number of 5-Star Reviews = 

Percentage of 5-Star Reviews = 

**Results for Unpaid Reviews for Musical Instruments**

## Summary
