# Amazon Vine Analysis 

## Background & Purpose of the Project

The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review. 

The purpose of the project is to analyze Amazon book reviews written by members of the paid Amazon Vine program, using PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, I will use PySpark to determine if there is any bias toward favorable reviews from Vine members in the dataset.

## Results

**How many Vine reviews and non-Vine reviews were there?**

**1.** The total Vine reviews is 4,781

![image](https://user-images.githubusercontent.com/108365182/196973912-3d4769bb-84a0-4fe1-8af0-e9459c27cae3.png)

**2.** The total non-Vine reviews is 332,395

![image](https://user-images.githubusercontent.com/108365182/196974012-3aad0252-5f39-44d5-aff9-54df2772a76b.png)

**How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?**

**1.** The total Vine reviews whith 5 stars is 1,604

![image](https://user-images.githubusercontent.com/108365182/196975063-1fa0ddce-ea40-46e7-b698-03fca7231855.png)

**2.** The total non-Vine reviews with 5 stars is 168,800

![image](https://user-images.githubusercontent.com/108365182/196975234-ad224011-ce9d-4461-93bd-af42b5cbf821.png)

**What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?**

**1.** The percentage of Vine reviews with 5 stars is 33.54%

![image](https://user-images.githubusercontent.com/108365182/196976487-b378a8ea-3fed-411c-b2e2-00d17522872e.png)

**2.** The percentage of non-Vine reviews with 5 stars is 50.78%

![image](https://user-images.githubusercontent.com/108365182/196976746-e0521f99-7ce3-4b7f-94a7-944ceeeab528.png)

## Summary

Based on our previous results, we can conclude that there is no bias toward favorable reviews from Vine members in the book category, as the percentage of total vine reviews with 5 stars is 33.54%, which it´s less than half of the total perecentage. Also, because it´s lower than the percentage of non-vine reviews with 5 stars, which is 50.78%.

To deepen this analysis I recommend analyzing another category related to humanities and literature, since in this type of category is quite difficult to find biases toward favorable reviews because is very personal and relataive, and compare it to another category such as technology, beauty, etc. 


