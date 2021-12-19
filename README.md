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
