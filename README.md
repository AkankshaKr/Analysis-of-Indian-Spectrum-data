# Analysis-of-Indian-Spectrum-data
Project Overview: In this project, I analyzed a spectrum auction dataset from India, which included information on 823 rows of spectrum auctions across 22 regions from 2010 to 2022. The dataset contained 57 variables, detailing various aspects of each auction, such as the year of the auction, participating bidders, awarded spectrum, and the price paid.
Steps Taken:
Data Cleaning and Preparation:
I started by loading the dataset into R for analysis. Using dplyr, I cleaned the dataset by removing irrelevant columns and duplicates. I also filtered and sorted the data to focus on meaningful insights such as region-wise and frequency band-wise trends.
I grouped the data by region and freqBand to summarize the number of occurrences of each frequency band being auctioned in different regions.
Exploratory Data Analysis (EDA):
For initial insights, I performed group-by analysis to identify patterns in the data. This was essential in understanding the distribution of spectrum auctions across different regions and frequency bands.
I also used visualization techniques like box plots and line graphs to assess the distribution of winning prices, reserve prices, and spectrum bands over time.
A heatmap was generated using ggplot2 in R to visualize the relationship between regions and frequency bands. This helped identify regions that were more active in specific spectrum bands.
Contingency Table and Heatmap:
Using the xtabs function, I created a contingency table to show how frequency bands were distributed across regions. I used ggplot2 to generate a heatmap, which visually represented the number of auctions across regions and frequency bands. The heatmap made it easier to identify high-activity regions and popular frequency bands.
Key Findings:
Through ratio analysis (winning price vs. reserve price), I identified that the 800-900 MHz frequency band was sold at the highest price in most regions, particularly in Madhya Pradesh, followed by Uttar Pradesh and Rajasthan.
I also found that the year 2015 was significant, as many high-priced auctions took place for the 800-900 MHz band that year. I used a treemap to highlight this trend, and subsequently isolated data from 2015 to perform a more in-depth analysis of specific regions and frequency bands.
Advanced Visualization in Tableau:
I also took the cleaned dataset to Tableau for further visualization. Using pivot tables and dynamic charts, I was able to display the trends more interactively. The treemap visualization in Tableau was particularly useful to represent the auction outcomes and frequency bands across different regions.
Challenges & Learnings:
A key challenge was ensuring that the data was accurately grouped and filtered, especially since multiple spectrum bands could be auctioned simultaneously. Handling this complexity required careful use of group_by functions in R.
I also had to ensure that all the visualizations were easy to interpret, which was crucial for presenting the findings to stakeholders.
