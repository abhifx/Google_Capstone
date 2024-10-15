# Data Analytics Capstone Project for Google Data Analytics Course
[Course: Google Data Analytics Capstone: Complete a Case Study](https://www.coursera.org/professional-certificates/google-data-analytics)

## Introduction
In pursuant of publishing a case study for data analytics assuming the role of a junior data analyst at a fictional company

## Quick links:
Data Source: divvy_tripdata [for 2023](https://divvy-tripdata.s3.amazonaws.com/index.html)
CSV files downloaded

## Data Visualizations: Power BI

Background
Goal: Understanding the cyclist data and then seeing the potential of converting casual cyclists to member cyclists.

## Data Source: 

Historical trip data to analyze and identify trends for the year 2023 which can be downloaded from divvy_tripdata. The data has been made available by Motivate International Inc.

This is public data that

### Data Organization: 
There are 12 files with the naming convention of YYYYMM-divvy-tripdata and each file includes information for one month, such as the ride id, bike type, start time, end time, start station, end station, start location, end location, and whether the rider is a member or not.

### Process
Power BI using power query is used to combine the data as Excel was unable to churn huge data (going beyond 1 million rows) plus cleaning CSV to xlsx format was tough job and resource hungry. 

### Data Exploration

Power BI: Each column was previewed and checked for the proper column type to proceed further.

# Observations:

The Ride ID is considered the primary key. However, since one year of data is used, no table combination was required. hence primary key role was stagnated to the counting of records.

The Data has null values in the start location and this could be replaced using latitude and longitude data, for this purpose, this is ignored. 
Th ride ID is the primary key and no duplicate value was found plus length of the ride ID (checked with len) was 16 and hence considered correct

The duration was separated and calculated as the difference between ride end time and ride beginning time. 

No columns were deleted however not all columns were used and could potentially be deleted. 

## Data Visualization: Power BI

First of all, member and casual riders are compared by the type of bikes they are using.

## Overall observation

![No. of rides](https://github.com/abhifx/Google_Capstone/blob/main/Number%20of%20Rides.png)

At a glance, it can be seen that there more rides by members than casual riders. the trend remains higher throughout the month. electric bike is mostly used with classic bikes near to it. curiously the docked bike is almost negligently used. we will see further that docked bikes are only used by casual bikers and members don't use the same. 

![ride based on bike type](https://github.com/abhifx/Google_Capstone/blob/main/ride%20by%20bike%20type.png)

electric bikes peaked at June while classic bikes peaked at August end. This probably is a seasonal impact but such data is not available for validation.

## Duration wise observation

![duration](https://github.com/abhifx/Google_Capstone/blob/main/duration.png)
When it comes to duration, Casual bike rides take the cake. so if we look at the last discussion, though members make more trips, duration-wise casual bikers do more. accordingly, classic bike usage increases which is the preferred mode by casual bikers.  

the casual riders ride more from period April to September. thus classic bike ride duration peaks at August, while electric bike peak at June-July period.

## weekly ride observation

![weekly data](https://github.com/abhifx/Google_Capstone/blob/main/weekly.png)

when looking at weekly data, members ride more during weekdays while casual bikers use more during weekends. this can be seen both in duration and number of rides. so the duration anomaly we have seen in the previous slide is caused by casual riders riding a lot more during the weekend. during the weekdays both casual and members ride the same duration.


# Conclusion:

Casuals are riding a lot less compared to members. However they not only ride for long, they also ride more during the weekends. 

# Suggestion:

1) Discontinue docked bikes to save cost because of negligible usage and is only used by casual users. thus generating no income.
2) Marketing campaigns might be conducted in spring and summer at tourist/recreational locations popular among casual riders.
3) Casual riders are most active on weekends and during the summer and spring, thus they may be offered seasonal or weekend-only memberships.
4) Casual riders use their bikes for longer durations than members. Offering discounts for longer rides may incentivize casual riders and entice members to ride for longer periods of time.
