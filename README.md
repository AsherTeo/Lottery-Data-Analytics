# Lottery Analysis with Dashboard 

## Table of Contents

1) [Overview](#overview)
2) [Objective](#objective)

## Overview
Welcome to the lottery data analysis project focusing on Toto, a popular lottery game in Singapore. The primary objective of this analysis is to uncover insights into the patterns and trends present in Toto draws over certain years. Specifically, we aim to identify 'hot' and 'cold' numbers, explore how often numbers from the previous draw reappear in subsequent draws and many more. 

The data is extracted from the official Singapore Pools [website](https://www.singaporepools.com.sg/en/product/Pages/toto_results.aspx) using `Selenium`, a web scraping tool. Then, we preprocess the data to extract relevant features such as winning numbers, draw dates, and additional information. We utilize **Python**, along with libraries such as `Pandas` and `Seaborn`, to conduct our analysis and gain insights from the Toto data. 

Moreover, we utilize `scipy` for statistical tests like the **t-test** and **Mann-Whitney U** test. These tests allow us to compare distributions of numerical features between different groups, aiding in our exploration of whether smaller sum, average, and standard deviation of Toto values are associated with better chances of winning the jackpot.

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
  
5) **Statics Analysis**: Additionally, we leverage scipy for statistical tests like the `t-test` and `Mann-Whitney U` test to compare distributions of numerical features between different groups, providing valuable insights into lottery patterns and trends.

6) **Interactive Dashboard**: The interactive Power BI dashboard facilitates analysis of hot and cold numbers, sortable by date, with hot numbers highlighted in red and cold numbers in blue for easy identification. Users can further refine their analysis by filtering for odd or even numbers and customizing the range of 10 to explore specific number pattern

</details>

## Exploratory Data Analysis (EDA)

1) **Identify "hot" and "cold" numbers**:
   
   ![image](https://github.com/AsherTeo/Lottery-Data-Analytics/assets/78581569/202b52a7-da84-45e1-89c1-f3722520c927)



   

 

<details>
  <summary>EDA</summary>

</details>
