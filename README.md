# PyBer_Analysis.

## Overview of the analysis: Explain the purpose of the new analysis.
PyBer is a ride sharing app company. They would like to analyze all the rideshare data from january to early May of 2019. This analysis will help PyBer improve access for the ride sharing services and determine affordability for under served neighborhoods
The goal of this analysis is to create a summary data frame of the ride sharing data by city type. The types of cities are Urban, Suburban and Rural. The data frame will include Total Rides, Total Drivers, Total fares, Avearge Fare per Ride, and Average Fare per Driver for all three types of cities.

### Resources:
city_data_csv - provides information such as the name of the city, driver count and type of the city (if it is urban, suburban or rural)
ride_data_csv - provides information on the city name with fare, ride ID and the date of ride
pyber_data = It is the merged dataframe from the city data and ride data


## Methods and Results: 
#### Total Rides: 
TotalRides was calculated using the groupby() function in the pyber_data_df dataframe (merged) to create a Series of data that has the type of city as the index, then apply the count() method to the "ride_id" column.

<img width="267" alt="image" src="https://user-images.githubusercontent.com/94877067/151283389-bf0d29de-0895-4521-b2fe-6b7bf3240b98.png">

##### RESULT:

<img width="88" alt="image" src="https://user-images.githubusercontent.com/94877067/151284594-2b60a4c6-388e-49bf-b1f7-93e8a17fe480.png">

Urban cities had more total rides and Rural cities had the least total rides.


#### Total Drivers:
Total drivers was calculated using the groupby() function in the city_data_df dataframe  to create a Series of data that has the type of city as the index, then apply the sum() method to the "driver_count" column.

<img width="278" alt="image" src="https://user-images.githubusercontent.com/94877067/151283731-6cfe32a7-8a73-474e-ba0f-66e6f713ba06.png">

##### RESULT:

<img width="133" alt="image" src="https://user-images.githubusercontent.com/94877067/151285040-c5d70a0e-3fab-4c2e-874c-2bc5a774e3f9.png">

Urban cities had more total Drivers and Rural cities had the least total drivers

#### Total Fares:
TotalFares was calculated using the groupby() function in the pyber_data_df dataframe (merged)  to create a Series of data that has the type of city as the index, then apply the sum() method to the "fare" column.

<img width="250" alt="image" src="https://user-images.githubusercontent.com/94877067/151283973-44f888aa-0a19-4734-8767-de6a14835233.png">

##### RESULT:

<img width="190" alt="image" src="https://user-images.githubusercontent.com/94877067/151285180-7c402f11-0909-4a83-b84b-199450693413.png">

Total fares was also high in urban city type as exected and Rural city type had the least

#### Average Fare per Ride: 
Average Fare was calculated by dividing the total fares for each city type with total rides for each city type.

<img width="245" alt="image" src="https://user-images.githubusercontent.com/94877067/151284027-c68f8b8a-ce31-4a00-bc31-c21599983de8.png">

##### RESULT:

<img width="296" alt="image" src="https://user-images.githubusercontent.com/94877067/151285296-c0b7cf42-4b1d-40c7-adc9-5c9e7ee6cc91.png">

Average fare per ride was high in rural city type and low in the urban city type


#### Averge Fare per Driver:  
Average Fare per driver was calculated by dividing the total fares for each city type with total drivers for each city type.

<img width="238" alt="image" src="https://user-images.githubusercontent.com/94877067/151284208-cb410021-b6df-431e-8ab6-2c485954312f.png">

##### RESULT:

<img width="344" alt="image" src="https://user-images.githubusercontent.com/94877067/151285568-f1f9445d-47fd-4f94-bae9-56c338575c8b.png">

Average fare per Driver was high in rural city type and low in the urban city type

The summary dataframe (PyBer summary) using all the above analysis was made.
Below is the code snippet for the summary dataframe

<img width="238" alt="image" src="https://user-images.githubusercontent.com/94877067/151284377-f1abdedc-313b-4f75-8f3c-e132380652ce.png">



<img width="362" alt="image" src="https://user-images.githubusercontent.com/94877067/151284301-1e47517b-7873-4f59-bdf6-6d8a08d36a1b.png">

## Summary:

As observed from the results above the three business recommendation for PyBer will include:

 - Access for the ride sharing services can be improved in the rural citi types  by increasing the number of drivers in those neighborhoods
 - Affordability in the rural neighborhoods can be improved by decreasing the fare per ride in rural city type that will allow more people in these neighborhood to use the ride sharing app.
 - Affordability in the rural neighborhoods can also be improved by decreasing the average fare per driver  in rural city type that will also allow more people in these neighborhood to use the ride sharing app.





