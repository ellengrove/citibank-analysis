# citibike-analysis
Citi Bike is a bike sharing system that serves the metropolitan New York City area. Publicly available ridership data from Citi Bike was used to identify and visualize trends in usage for one week in April 2022. The main objectives of this analysis was to evaluate patterns in ridership on weekdays versus weekends and between two different types of Citi Bike users: subscribers and casual riders. 

# Data Source
See https://ride.citibikenyc.com/system-data for a description of the data that Citi Bike publishes. Individual .csv files can be downloaded from https://s3.amazonaws.com/tripdata/index.html. 

# Data Processing
The data was in largely workable format straight from Citi Bike's website. Instead of using an entire month's worth of trip data, a smaller weeklong subset was selected for purposes of this analysis (April 3, 2022 - April 9, 2022). Rows with null values were removed. Additionally, rides with trip durations lasting zero minutes or less or greater than 2 hours were removed from analysis (see, https://help.citibikenyc.com/hc/en-us/articles/360032024912-How-long-can-I-keep-a-bike-out-; rides greater than 2 hours are assumed to be extreme outliers and rides shorter than zero minutes are assumed to be erroneous).

# 