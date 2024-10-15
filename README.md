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


Prepare
Data Source: Historical trip data to analyze and identify trends for the year 2023 which can be downloaded from divvy_tripdata. The data has been made available by Motivate International Inc.

This is public data that

###Data Organization: There are 12 files with naming convention of YYYYMM-divvy-tripdata and each file includes information for one month, such as the ride id, bike type, start time, end time, start station, end station, start location, end location, and whether the rider is a member or not.

###Process
Power BI using power query is used to combine the data as Excel was unable to churn huge data (going beyond 1 million rows) plus cleaning CSV to xlsx format was tough job and resource hungry. 

###Data Exploration

Power BI: Each column was previewed and checked for the proper column type to proceed further.

Observations:

The Ride ID is considered the primary key. however since one year of data is used, no table combination was required. hence primary key role was stagnated to counting of records.

The Data has null values in start location and this could be replaced using latitude and longitude data, for this purpose, this is ignored. 
Th ride ID is the primary key and no duplicate value was found plus length of the ride ID (checked with len) was 16 and hence considered correct

The duration was separated and calculated as the difference between ride end time and ride beginning time. 

No columns were deleted however not all columns were used and could potentially be deleted. 


Data Analysis
Data Visualization: Power BI

First of all, member and casual riders are compared by the type of bikes they are using.

![No. of rides](https://github.com/abhifx/Google_Capstone/blob/main/Number%20of%20Rides.png)
image

The members make 59.7% of the total while remaining 40.3% constitutes casual riders. Each bike type chart shows percentage from the total. Most used bike is classic bike followed by the electric bike. Docked bikes are used the least by only casual riders.

Next the number of trips distributed by the months, days of the week and hours of the day are examined.

image image

Months: When it comes to monthly trips, both casual and members exhibit comparable behavior, with more trips in the spring and summer and fewer in the winter. The gap between casuals and members is closest in the month of july in summmer.
Days of Week: When the days of the week are compared, it is discovered that casual riders make more journeys on the weekends while members show a decline over the weekend in contrast to the other days of the week.
Hours of the Day: The members shows 2 peaks throughout the day in terms of number of trips. One is early in the morning at around 6 am to 8 am and other is in the evening at around 4 pm to 8 pm while number of trips for casual riders increase consistently over the day till evening and then decrease afterwards.

We can infer from the previous observations that member may be using bikes for commuting to and from the work in the week days while casual riders are using bikes throughout the day, more frequently over the weekends for leisure purposes. Both are most active in summer and spring.

Ride duration of the trips are compared to find the differences in the behavior of casual and member riders.

image
image

Take note that casual riders tend to cycle longer than members do on average. The length of the average journey for members doesn't change throughout the year, week, or day. However, there are variations in how long casual riders cycle. In the spring and summer, on weekends, and from 10 am to 2 pm during the day, they travel greater distances. Between five and eight in the morning, they have brief trips.

These findings lead to the conclusion that casual commuters travel longer (approximately 2x more) but less frequently than members. They make longer journeys on weekends and during the day outside of commuting hours and in spring and summer season, so they might be doing so for recreation purposes.

To further understand the differences in casual and member riders, locations of starting and ending stations can be analysed. Stations with the most trips are considered using filters to draw out the following conclusions.

image

Casual riders have frequently started their trips from the stations in vicinity of museums, parks, beach, harbor points and aquarium while members have begun their journeys from stations close to universities, residential areas, restaurants, hospitals, grocery stores, theatre, schools, banks, factories, train stations, parks and plazas.

image

Similar trend can be observed in ending station locations. Casual riders end their journay near parks, museums and other recreational sites whereas members end their trips close to universities, residential and commmercial areas. So this proves that casual riders use bikes for leisure activities while members extensively rely on them for daily commute.

Summary:

Casual	Member
Prefer using bikes throughout the day, more frequently over the weekends in summer and spring for leisure activities.	Prefer riding bikes on week days during commute hours (8 am / 5pm) in summer and spring.
Travel 2 times longer but less frequently than members.	Travel more frequently but shorter rides (approximately half of casual riders' trip duration).
Start and end their journeys near parks, museums, along the coast and other recreational sites.	Start and end their trips close to universities, residential and commercial areas.
Act
After identifying the differences between casual and member riders, marketing strategies to target casual riders can be developed to persuade them to become members.
Recommendations:

Marketing campaigns might be conducted in spring and summer at tourist/recreational locations popular among casual riders.
Casual riders are most active on weekends and during the summer and spring, thus they may be offered seasonal or weekend-only memberships.
Casual riders use their bikes for longer durations than members. Offering discounts for longer rides may incentivize casual riders and entice members to ride for longer periods of time.
