# Amazon Vine Review Analysis
## Analysis with Pyspak and AWS

## Project Overview
For this project I am using Amazon’s cloud service AWS, Google Colab and Pyspark to analyze Amazon’s reviews for outdoor products. The purpose of this analysis is to determine if there is any bias toward favorable reviews from Vine members. Amazon Vine program is a service that allows manufacturers to have reviews posted on Amazon for their pre-release items, for an additional fee.

## Results
In this analysis I analyzed reviews that have more than 20 total votes and the percentage of helpful votes is equal or greater than 50.

### How many Vine reviews and non-Vine reviews were there?

There were

107 Vine reviews and
39,869 non-Vine reviews.

![image](https://user-images.githubusercontent.com/95595378/165026412-4d12ffda-b7e8-4b5d-bdcc-307cabf13387.png)

Figure 1: Total Vine and non-Vine reviews.

### How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?

There were

56 five stars Vine reviews and
21,005 five stars non-Vine reviews.

![image](https://user-images.githubusercontent.com/95595378/165026701-b410b8ab-46ce-4691-99d2-2150f6ccdc82.png)

Figure 2: 5-star Vine and non-Vine reviews.

### What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

52.34 % of Vine reviews were 5 stars and
52.69 % of non-Vine reviews were 5 stars.

![image](https://user-images.githubusercontent.com/95595378/165026371-5ff08a92-8930-4694-a817-084b4a7a53c0.png)

Figure 3: Percentage of 5-star Vine and non-Vine reviews.

## Summary
The purpose of this analysis is to analyze and determine if there is any bias toward favorable reviews from Vine members in the dataset. I analyzed reviews that have more than 20 total votes and the percentage of helpful votes is equal or greater than 50. This selection was made in order to pick reviews that are more likely to be helpful.

### Positivity bias for reviews in the Vine program

In the analysis I analyze 5-star reviews within conditions mentioned above. Calculations show that there is no positivity bias for reviews in the Vine program. The results show that percentage of 5 stars Vine reviews is 52.34% and percentage of 5 stars non-Vine reviews is 52.69%. Non-Vine reviews have slightly higher percentage of the 5 stars reviews, 0.35% percentage points to be exact.

### Additional analyses and suggestions

We could expand this analysis by calculating percentage for all stars reviews. Based on the results (Figure 4), there is a larger difference in percentage for 1-star reviews than for 5-stars reviews. Vine reviews have only 0.93% of 1-star reviews, while non-Vine reviews have 13.35 % 1-star reviews within conditions mentioned above. Similarly, there is 1.87% 2-stars Vine reviews and 6.05% 2-stars non-Vine reviews.

![image](https://user-images.githubusercontent.com/95595378/165026286-88c33e0f-3d29-4b15-b2ec-e3a45ac2c72e.png)

Figure 4: Summary table for all star reviews.

The results show that there could be positivity bias for reviews in the Vine program, when looking from 1 and 2-star reviews perspective.

Additionally, I would suggest another analysis beyond the given dataset. Non-vine reviews outnumber Vine reviews for 37,260 % (in this dataset, within certain conditions). In this case Vine reviews won’t affect the overall rating of the items. On Amazon site for Vine reviews https://www.amazon.com/gp/vine/help we can find explanation about the Vine program. The first sentence states: “Amazon Vine invites the most trusted reviewers on Amazon to post opinions about new and pre-release items to help their fellow customers make informed purchase decisions (1).” Vine reviews could have impact on newly released items sold on Amazon. For the manufacturers might be beneficial to have some reviews posted when launching their newly released products. At this point I would suggest to perform analysis on items that are similar (one group with Vine reviews and the other without) and measure sales increase over time. Based on that we could observe if Vine reviews contributed to faster increase of the sales of newly released items.

