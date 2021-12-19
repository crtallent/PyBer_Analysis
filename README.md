# PyBer_Analysis

## Overview of PyBer Analysis
For this project, I was tasked with creating a summary DataFrame of PyBer's ride-sharing data by city type.  The goal was to get an in-depth comparison between average weekly fares for three city types.  This analysis was completed using data from PyBer ride-sharing data in 2019.  The three city types are as follows:

* Rural Cities
* Suburban Cities
* Urban Cities

![Ride_Sharing_Data](https://github.com/crtallent/PyBer_Analysis/blob/main/Analysis/Fig1.png)













The goal is to determine how the data differs according to city type, so that the decision-makers at PyBer can determine if they need to make strategic changes on how the company operates.  Additional data that was analyzed prior to this project includes:

* Number of rides per city
* Number of drivers in each city
* Date and time of fares in each city
* Mean, median and mode for ride counts per city type
* Average (median) fares per city type



![Fares_per_city_type](https://github.com/crtallent/PyBer_Analysis/blob/main/Analysis/Fig5.png)

```
ride_percents = 100 * pyber_data_df.groupby(["type"]).count()["ride_id"] / pyber_data_df["ride_id"].count()
ride_percents
```


## Resources
- Data Sources: city_data_csv, ride_data_csv
- Software: Python 3.7.11, Jupyter NOtebook 7.29.0

## PyBer Analysis Results
Upon analyzing the data, there are many differences between the three city types.  As one might expect with differing population levels between rural, suburban, and urban city types, the total rides for the urban cities was signifantly higher than both the suburban and rural areas.  This is also true of the number of total drivers and and total fares. However, the average fare per ride and per driver were lower in urban areas than in suburban and rural areas.

![pyber_summary_df](https://github.com/crtallent/PyBer_Analysis/blob/main/Analysis/summary.png)

The following is indicated by this data:

* There were slightly over 2 1/2 times more rides completed in urban cities than suburban cities, and 5 times more rides completed in suburban cities than rural cities
* There were roughly 5 times more drivers in urban cities than suburban cities, and 6 times more drivers in suburban cities than rural cities
* The total fares earned were roughly double in urban cities than in suburban cities, and roughly 4 1/2 times more than total fares in rural cities.
* The average fare per ride was $24.53 in urban areas; however, this amount increased in suburban areas with $30.97, and in rural areas with $34.62.
* The average fare per driver was $16.57 in urban areas; however, this amount nearly doubled in suburban areas, and tripled in rural areas.

![total_fare_by_city_type](https://github.com/crtallent/PyBer_Analysis/blob/main/Analysis/total_fare.jpg)

## PyBer Summary

Upon analysis of this data, there are some areas that could be looked at further.  One recommendation would be to look at urban city fare amounts, as the average fare per ride and per driver are much lower than in suburban and rural areas.  Another recommendation would be to look into getting more drivers in underserved areas, such as suburban and rural areas.  Finally, since fares are much higher in rural areas than in suburban and urban areas, decreasing fares may increase the amount of rides completed.
