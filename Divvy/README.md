# Divvy Trips Case Study

## Table of Contents
- [`Introduction`](#introduction)
- [`Process`](#process)
- [`Findings`](#findings)
    - [`General`](#general)
    - [`Traffic`](#traffic)
    - [`Ride Duration`](#ride-duration)
    - [`Ride Distance`](#ride-distance)

## Introduction  
<p>Divvy is a bicycle sharing system in Chicago. There are two types of customers using Divvy's Bike-sharing service: <strong>casual users</strong> and <strong>annual members</strong>. Annual members are much more profitable than casual users.</p>
<p><strong>Goal: </strong>explore data and find insights in order to develop strategies to convert casual riders to annual members</p>
<p><strong>About data: </strong>the last 6 months' trip data uploaded by Divvy (April-September 2021). <a href='https://divvy-tripdata.s3.amazonaws.com/index.html'>Website</a></p>

## Process  
1. [`Get the dataset`](https://divvy-tripdata.s3.amazonaws.com/index.html)
2. [`Clean and transform the data`](https://github.com/serkansalcan/analytics-projects/blob/main/Divvy/data_cleansing.ipynb)
3. [`Perform Exploratory Data Analysis`](https://github.com/serkansalcan/analytics-projects/blob/main/Divvy/exploratory_data_analysis.ipynb)
4. [`Create a Tableau Dashboard`](https://public.tableau.com/views/DivvyTrips_16357928926750/Dashboard?:language=en-US&:display_count=n&:origin=viz_share_link)

## Findings
### General
- 55.4% trips done by annual members, 44.6% by casual users  
![image](https://user-images.githubusercontent.com/27378210/147408155-3c57e13b-4938-46bd-8458-d1812cc73e67.png)  
- Both annual members and casual users used classic bikes more, compared to electric bikes.  
![image](https://user-images.githubusercontent.com/27378210/147408182-efa31c60-406e-48dc-b083-ad7d312154a2.png)
- Users generally take bikes in one location and return it to another location. Only 5.57% of trips return the same location.  
![image](https://user-images.githubusercontent.com/27378210/147408192-9854367a-4f28-4852-a7c3-25ce2a126f20.png)  
- Correlations:  
![image](https://user-images.githubusercontent.com/27378210/147408217-ee9755a2-a446-4744-874b-0beefd5a0718.png)  
There is a positive correlation (low degree, <0.3) between ride distance and ride duration, r=.22.  

### Traffic  
- During the day:  
    - Both member and casual users creates the most traffic between 12:00 and 19:00. The traffic gets its peak at 17:00 for both.  
    - Annual members' traffic peaks at 08:00 and 17:00, which are the start and end of business hours. There is no peak for casual users at 08:00.  
    ![image](https://user-images.githubusercontent.com/27378210/147497101-ba63797f-bd12-4a79-85fb-43ba1af65940.png)
- Days of Week:  
    - The number of trips by casual users is low during weekdays and starts to increase by Friday and peak at Saturday.  
    - Annual members are almost opposite of that. It is higher during weekdays and their demand decreases at weekend. 
    ![image](https://user-images.githubusercontent.com/27378210/147496279-3a6b2080-a5cb-411e-8865-373a2f007c93.png)    
- Traffic by Stations:  
    - There are 773 stations, but almost half of the traffic comes from the top 100 stations.
    - Top 100 stations are not exactly the same for annual members and casual users. 78 of them are the same. 22 stations are  different.  

### Ride Duration  
- Casual users ride bikes longer than annual members.  
- Casual users ride classic bikes for longer duration compared to electric bikes.
![image](https://user-images.githubusercontent.com/27378210/147504207-77a2384d-389f-4ab0-9109-78d2a35ed6ad.png)  
- Ride duration gets longer during weekends for both user types.  
![image](https://user-images.githubusercontent.com/27378210/147504222-66ff6451-5813-4913-97e6-7bffd7308296.png)  

### Ride Distance  
- No significant difference between annual members and casual users.  
- Both user types travel relatively longer distances with electric bikes, compared to classic bikes.  
![image](https://user-images.githubusercontent.com/27378210/147504045-c36459c6-758f-4dab-bff4-57be301b9aa7.png)  
