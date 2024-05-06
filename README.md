# Lottery Analysis with Dashboard 

## Table of Contents

1) [Overview](#overview)
2) [Objective](#objective)
3) [Key Features](#key-features)
4) [Exploratory Data Analysis ](#exploratory-data-analysis )

## Overview
Welcome to the lottery data analysis project focusing on Toto, a popular lottery game in Singapore. The primary objective of this analysis is to uncover insights into the patterns and trends present in Toto draws over certain years. Specifically, we aim to identify 'hot' and 'cold' numbers, explore how often numbers from the previous draw reappear in subsequent draws and many more. 

The data is extracted from the official Singapore Pools [website](https://www.singaporepools.com.sg/en/product/Pages/toto_results.aspx) using `Selenium`, a web scraping tool. Then, we preprocess the data to extract relevant features such as winning numbers, draw dates, and additional information. We utilize **Python**, along with libraries such as `Pandas` and `Seaborn`, to conduct our analysis and gain insights from the Toto data. 

Moreover, we utilize `scipy` for statistical tests like the **t-test** and **Spearman's rank** correlation. These tests allow us to compare distributions of numerical features between different groups, aiding in our exploration of whether smaller sum, average, and standard deviation of Toto values are associated with better chances of winning the jackpot.

Additionally, we've enhanced our analysis by building an interactive dashboard using **Power BI**. This dashboard provides a fun and engaging way for our audience to interact with the Toto data, similar to the experience of being in a casino. Inspired by casino games like roulette, where players can view statistics on red and black winning rates or the last 10 numbers, our dashboard offers dynamic visualizations and statistics on Toto draws. It allows users to explore trends, patterns, and insights in an interactive and entertaining manner.

## Objective

1) **Identify "hot" and "cold" numbers**: Analyze historical data to determine which numbers have appeared most frequently (hot numbers) and least frequently (cold numbers) in past draws.
   
2) **Frequency of numbers from the previous draw in subsequent draws**: Quantify how often numbers from the previous draw are repeated in subsequent draws, exploring any patterns or trends in their recurrence.
   
3) **Consecutive number occurrence in winning combinations**: Investigate whether consecutive numbers, such as 12 and 13, are more or less likely to appear together in winning combinations compared to non-consecutive numbers.
<details>
   <summary>See More</summary>  
   
4) **Patterns of number selection**: Explore whether certain numbers tend to be selected together more frequently than others, indicating potential patterns or strategies used by players.
5) **Balance of odd and even or high and low numbers**: Analyze the distribution of odd and even numbers, as well as high and low numbers, in winning sets to determine if there are any biases or patterns in their occurrence.
   
6) **Relationship between Toto values and jackpot chances**: Investigate whether specific characteristics of Toto values, such as smaller or larger sums, averages, and standard deviations, are associated with an increased likelihood of winning the jackpot.
    
7) **Temporal analysis of winners**: Determine which years, months, and days of the week have historically had the highest total number of winners, identifying any temporal patterns or trends.
    
8) **Correlation among winning numbers**: Explore if winning numbers exhibit any correlations or tendencies to appear together more frequently than expected by chance, indicating potential patterns in number selection or drawing mechanisms.
   
</details>

## Key Features

1) **Lottery Dataset Extraction**: Utilize `Selenium` to extract lottery data from the official Singapore Pools website. Ensure that the dataset covers a substantial period, from March 1, 2021, to February 29, 2024, providing a rich source of data for analysis.
            
2) **Data Wrangling**: Perform data cleaning tasks such as handling missing values, replacing '-' with 0, and removing any unnecessary characters like '$'. Additionally, ensure that the data types are correctly specified for further analysis.
<details>
   <summary>See More</summary>
   
3) **Feature Engineering**: Create new columns to enhance the dataset's analytical capabilities, including columns for:
    - Sum, Average, and Standard Deviation of Numbers drawn on each draw date, providing insights into the distribution of numbers.
    
    - Occurrences of Numbers within Specific Ranges (e.g., '1-9', '10-19', '20-29', '30-39', '40-49'), enabling analysis of number distribution patterns.
    
   - Occurrences of Repeated Numbers from Previous Draws
    
   - Occurrences of Consecutive Numbers from each draw (e.g 12, 13 or 35, 36)
  
 
4) **Data Analysis**: For data analysis, utilize `Seaborn` to visualize number distribution, correlations, and consecutive number pairs' frequencies in winning combinations.
  
5) **Statics Analysis**: Additionally, we leverage scipy for statistical tests like the `t-test` and `Spearman's rank` correlation to compare distributions of numerical features between different groups, providing valuable insights into lottery patterns and trends.

6) **Interactive Dashboard**: The interactive Power BI dashboard facilitates analysis of hot and cold numbers, sortable by date, with hot numbers highlighted in red and cold numbers in blue for easy identification. Users can further refine their analysis by filtering for odd or even numbers and customizing the range of 10 to explore specific number pattern

</details>

## Exploratory Data Analysis 

**1)** **Identify "hot" and "cold" numbers**:
   
![image](https://github.com/AsherTeo/Lottery-Data-Analytics/assets/78581569/e32a097d-f179-4b3f-899d-406942d9c262)

The "hot" and "cold" numbers are identified from the lottery dataset spanning from 01 March 2021 to 29 February 29 2024. The top 5 hot numbers, namely **44**, **28**, **49**, **1**, and **37**, demonstrate higher occurrence frequencies, while the least 5 numbers, including **39**, **29**, **33**, **14**, and **9**, appear less frequently. It's important to note that these results may vary depending on the date range analyzed

**2)** **Frequency of numbers from the previous draw in subsequent draws**:

![image](https://github.com/AsherTeo/Lottery-Data-Analytics/assets/78581569/7069ad0c-f1a0-4329-9c12-7991d7ee8107)

Around 45% of 1 repeated numbers appear from the previous draw, 29% show 0 repetitions, 20.4% have 2 repetitions, and 5% have 3 or more repetitions. This suggests that there is close to a 50% chance that one number out of the seven numbers from the previous draw will appear in the next draw, indicating a potential strategy of randomly picking one.

**3)** **Consecutive number occurrence in winning combinations**:

![image](https://github.com/AsherTeo/Lottery-Data-Analytics/assets/78581569/d245046b-d493-4ddb-aeb0-505fa998d355)

53% of draws do not have any consecutive numbers, while 34% have one consecutive number, and 12.1% have two consecutive numbers. This analysis reveals that there is only a 1/3 chance that a winning combination will include one consecutive number pair (e.g., 12 and 13). 

<details>
  <summary>See More </summary>

**4)** **Patterns of number selection**:

2-Gram:
![image](https://github.com/AsherTeo/Lottery-Data-Analytics/assets/78581569/1ca194c5-88cd-4188-9fd2-b545cc36c783)

The top 5 2-grams are **(23,24), (44,45), (38,41), (18,24)**, and **(28,31)**.

3_Gram:
![image](https://github.com/AsherTeo/Lottery-Data-Analytics/assets/78581569/b9f0ca98-eac6-43b9-9042-672cfc792fa2)

The top 5 3-grams are **(28,31,37), (24,26,28), (16,17,20), (31,32,33)**, and **(3,7,9)**.

**5)** **Balance of odd and even or high and low numbers**:

![image](https://github.com/AsherTeo/Lottery-Data-Analytics/assets/78581569/2ff3d743-bdc1-4bc5-96b4-6694d3848c4d)

The distribution of odd and even numbers is approximately equal, with each occurring around 50% of the time. Similarly, there's a balanced distribution between low and high numbers.

Interestingly, the probability of selecting a combination with an equal mix of odd and even numbers, such as 20-20, is slightly higher than that of other combinations, accounting for approximately 21.1% of occurrences.
   
**6)** **Relationship between Toto values and jackpot chances (T-Test)**:

**Null Hypothesis(H0)**: A smaller sum, average, and standard deviation (SD) of Toto values do not affect the chance of winning the jackpot.

**Alternative Hypothesis (H1)**: A smaller sum, average, and standard deviation (SD) of Toto values are associated with a better chance of winning the jackpot


|                   |  p-values |  
|-------------------|------------|
| Sum               |  0.01096054	 |
| Average           |  0.01096054	 | 
| Standard Deviation | 0.5925751  | 

The p-values for the sum and average of Toto values are both less than 0.05, indicating strong evidence to reject the null hypothesis for these variables. This suggests that a smaller sum or average of Toto values is indeed associated with an increased likelihood of winning the jackpot, supporting the alternative hypothesis.

Conversely, the t-statistic for the standard deviation of Toto values is not statistically significant, with a p-value greater than 0.05. Therefore, we cannot reject the null hypothesis, indicating that there's no notable difference in the standard deviation of Toto values between draws with and without first prize winners.

**7)** **Temporal analysis of winners**:

![image](https://github.com/AsherTeo/Lottery-Data-Analytics/assets/78581569/8abcd009-48b2-4734-9b6b-c7287c17f9c7)

By the year 2023, there were the most occurrences of 55. In terms of months, January had the highest count, with 19 instances. Lastly, when considering individual days, Monday stood out with a total count of 76.

January tends to have the highest number of winners due to the fact that grand prizes, often ranging from 5 million to 10 million, are frequently scheduled for January, coinciding with events such as New Year's and Chinese New Year. Furthermore, these grand prize draws commonly occur on Fridays.

**8)** **Correlation among winning numbers (Spearman's rank correlation)**:

![image](https://github.com/AsherTeo/Lottery-Data-Analytics/assets/78581569/b577f073-7646-479b-ac09-57b49bb73728)

The heatmap indicates some correlations between pairs of winning numbers, particularly when draws are sorted from small to large. However, in live Toto draws where numbers are randomly selected, such structured arrangement does not exist, leading to less pronounced correlations. As a result, predicting or analyzing the relationships between winning numbers becomes more challenging. Thus, this correlation may not hold true for live Toto draws due to the lack of a consistent arrangement.

</details>


