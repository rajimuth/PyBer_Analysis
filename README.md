# PyBer_Analysis.
The analysis should contain the following:
### Resources:
city_data_csv - provides information such as the name of the city, driver count and type of the city (if it is urban, suburban or rural)
ride_data_csv - provides information on the city name with fare, ride ID and the date of ride
pyber_data = It is the merged dataframe from the city data and ride data

## Overview of the analysis: Explain the purpose of the new analysis.
PyBer is a ride sharing app company. They would like to analyze all the rideshare data from january to early May of 2019. This analysis will help PyBer improve access for the ride sharing services and determine affordability for under served neighborhoods
The goal of this analysis is to create a summary data frame of the ride sharing data by city type. The types of cities are Urban, Suburban and Rural. The data frame will include Total Rides, Total Drivers, Total fares, Avearge Fare per Ride, and Average Fare per Driver for all three types of cities.

Methods: 
Total Rides: TotalRides for calculated using the groupby() function to create a Series of data that has the type of city as the index, then apply the count() method to the "ride_id" column.


The purpose of the analysis is to 
Results: Using images from the summary DataFrame and multiple-line chart, describe the differences in ride-sharing data among the different city types.
Summary: Based on the results, provide three business recommendations to the CEO for addressing any disparities among the city types.