# Amazon_Vine_Analysis
Module 16

### Overview of the Analysis
Our client, SellBy, has asked us to analyze Amazon reviews written by members of the paid Amazon Vine program.  The Amazon Vine program is intended to allow manufacturers to receive reviews of their products.  Companies, like SellBy, pay for the Amazon Vine service.  The purpose of the the analysis is to discover if the reviewers from Vine are skewed in such a way as to write favorable reviews for the products because they are paid.  Our analysis will show that this concern over being unrealistically positive is not necessarily the case, but the arguement can be made that for SellBy to pay for such a service is unnecessary in the first place.

### Results
We chose Amazon Reviews of Books as our data source to take this deeper dive into Vine reviews.  The following DataFrame shows they type of data that we were working with;
![total data](https://user-images.githubusercontent.com/85403978/135722240-b7b707f4-df2a-4e58-be00-828b373edb2b.png)

In this data of over 3,000,000 titles, only two titles had a Vine Review!  Which begs questions as to the necessity of Vine in the first place since they write so few reviews to begin with.

![image](https://user-images.githubusercontent.com/85403978/135722364-eaeae4db-1883-4fbf-9f82-efdff2033395.png)

Along with the reviews, the reviewer can assign a "Star" rating to visually demonstrate their overall opionion of the book (5-Stars being the best, or most favorable).  Of the two Vine reviews in the entirety of the DataFrame, one was a 5-Star review.  Hence, 50% of the Vine reviews had the most favorable rating.  On the contrary, we filtered the non-Vine reviews based on records with 20 votes or more, and a "helpful_votes" ratio of 50% or more.  As a result, we're left with over 400,00 reviews that are not associated with Vine.  Of that count, 242,889 reviewers left 5-Star ratings, or over 60%.

![image](https://user-images.githubusercontent.com/85403978/135722893-21582ca2-b1c6-4e42-a271-536e35a8bf44.png)


### Summary
As you can see by the data, the original question of whether or not Vine reviews are skewed positive, is almost irrelevant.  The data shows that a Vine review has a 50/50 chance of leaving 5-Stars, but out of only two reviews, I'd say that there isn't enough participation (isn't enough data) to make that determination.  The reviews that did not come from Vine were over 60% most favorable.  There is plenty of data there to say that the reactions are valid but to make a comparison to Vine reviews, there isn't enough information to go on.  The greater question is why would someone pay for a service that only offers two reviews in a data set this size?  My recommendation to SellBy is to stop paying for the Vine service.
