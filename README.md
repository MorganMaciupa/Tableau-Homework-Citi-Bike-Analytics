
# Tableau-Homework-Citi-Bike-Analytics

## Data Selection and Clean Up
Data csv files were selected from February, May, August and Novemeber in 2021 as a means of representing each of the four seasons within on calendar year. In real-world application, each of the 12 months of data would be utilised however Tableau Public will not handle more than 15,000,000 rows of data. 

CSVs were first imported and checked for data types, which revealed that in some datasets, the start and end station ID numbers were stored as integers, while others were stored as strings. To overcome the handling issues in Tableau that would have resulted, the above columns were all imported as string data (that is, in words as opposed to numbers). 

Data types were then checked for consistency across all datasets, and merged in to one dataframe. 

Further data cleaning was required to convert the depreciated bike type term from 'docked bikes' used in older datasets February and May to 'classic bike'. 

Columns containing data that was not utilised in the analysis were removed to scale down the size of the dataframe, and unwanted spacing was removed from station names. 

## Limitations of Dataset
There were some limitations of the dataset used, which limited the number of visulaisations that were created. These included:
- Data did not contain rider details which would have been used to identify growth in ridership over 2021 period. 
- Data on the number of electric bikes in the Citi Bike's New York fleet is unavailable, and the percentage of electric bike rides and classic bike rides does not represent the difference in size of fleet. 

## Dashboard Analysis
### Dynamic Map

A map over New York City was generated showing the total usage figures of ride start stations over the four selected months in 2021. This can be broken down by month, and shows that the most popular stations do not vary greatly throughout the year.

### Usage Dashboard
This dashboard illustrates the number of trips taken over different time periods. 

The pie chart displays the number of trips taken during the week (ie Monday - Friday) vs the number of trips taken over the weekend. We can see that, although the weekend accounts for 28.57% of the days of the week (ie, 2 out of 7) the total usage figures for the weekend are only 26.90%, outlining that less rides are taken over the weekend period. 

Broken down by hour, we can see that most rides are taken during the week at peak traffic hours of 8am and 5-6pm, which indicates that this is a popular means of transport too and from work, or while road traffic is at its peak. More data could be collect on ride purpose to further detail this phenomenon. 

Breaking the total number of rides taken down in to months, it is concluded that Citi Bike rides are 4-5x more popular in summer months (ie, August, 3 072 833 total rides) than they are in winter (February, 649 983 total rides). Spring time (May, 2 724 165 total rides) is a close second most popular season. 

### Start Station Dashboard

This dashboard outlines the most and least popular start stations for Citi Bike rides in New York City for month month of each season in the year 2021.

We can see that while the 10 most popular start stations do not vary month to month (or season to season), the total usage of each station, and their place in the top 10 does change. 

There are some dummy stations within the bottom 10 that are used by staff, and as a result the bottom 10 stations listed do not truly represent the 10 least popular stations with in the Citi Bike NY City program. 

