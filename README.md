# Cyclistic Bike Share Analysis 

 Hi, Join me in the Google Data Analyst Capstone Project, focusing on the Cyclistic Bike Share Case Study! 
 In this case study I will be analyzing a public dataset for a fictional company provided by the course.

In this case study , we  dive deep into data analysis, applying advanced techniques to extract meaningful conclusions. Explore the intersections of the Cyclistic Bike Share Case Study and the principles of the Google Data Analyst Professional Certificate, solidifying  our skills in interpreting and presenting data.


**Dataset**
 I Use Cyclistic’s historical trip data to analyze and identify trends.e Cyclistic
is a fictional company. For the purposes of this case study, the datasets are appropriate and
will enable me to answer the business questions. The data has been made available by
Motivate International Inc. under this license (https://www.divvybikes.com/data-license-agreement.)

**Tools**
*R* - Data Analysis
.*PowerBI* - Creating reports

**Limitations**
I had to remove all null values from data because they would have affected the accuracy of my conclusions from the analysis. .
I had to remove some columes i dont need in my analysis.
Ihad to delete rows with negative values in duration column. 

### BUSINESS QUESTIONS
1- How do casual and  member riders use Cyclistic Bike Share diferently.
2- Why would casual rides buy annual Cyclistic  memberships.
3-How can Cyclistic use digital media to influence casual riders to become members.
 For this project ,I will focouse on the first busnis question and then i will do the second and thierd one.

### BUSINES Task
Cyclistic bike share company based in Chicago,reccognizes the importance of increasing the number of annual subscribers for its future success.To achieve this goal,this project aims 
to analyze the differences in bike usage between casual riders and annual members and develop anew marketing strategy to convert casual riders in to annual subscribers.led by lily Morenothe director of marketing, and supported by Cyclistic;s markiting analytics team,this project will collect analyze and report data to guide the company;smarketing strategy.

##*Data Preparation*

I use primary source data downloaded from Cyclistic;s internal data mwhich is made available by divvy open source data.The available data will allow for examination of differences between user types, but not identification of underlying reasons.

Data has been downloaded(12.Csv files were downloaded from 1 jan 2020 to 31 Dec 2020) and copies have been stored securely on my computer.
these files were import to R Studio using read_csv function .The 12 downloaded  Csv files were merged into a master Data named *all_trips*

##*Data Processing*

 Iused  RStudio Desktop  as the data processing tool. the master data was fed into the software as a data sourse and transfomed .
 Handling missing values.
 Data cleaning and formatting.
We will want to add some additional columns of data such as 
day ,month ,year  that provide additional  opportunities to aggregate the data.
then i combined all 12 csv files into one file named *all_trips*
We will want to add acalculated field for length of ride since the data 
did not have the tripduration coulumn,We will add ride_length to column to the data .
There are some rides where tripduration shows up as negative,where Divvy took bikes 
out of circulation for quality control reasons.we will want too delet these rides.

##*Data Analysis* 

Data has been cleaned and now we will move toward the analysis process

the analysis was performed using R code 

 **CONDUCT DESCRIPTIVE ANALYSIS  on *ride_length (all figures in seconds)***

##### Summary of ride_length:_

![Screenshot (134)](https://github.com/nisrinfrh/google_project/assets/157531427/351f8af9-00f5-4bcc-b950-2b36526adc39)

##### Compare members and casual users:_
![Screenshot (135)](https://github.com/nisrinfrh/google_project/assets/157531427/dd3f856d-bb6c-4137-8e95-7dbe70a9a056)
  
#### See the average ride time by each day for members vs casual users:

![Screenshot (137)](https://github.com/nisrinfrh/google_project/assets/157531427/0522f602-1584-4a6d-bca9-a3ae9a6772ba)

##### Analyze ridership data by type and weekday
*#calculates the number of rides and average duration*

![Screenshot (140)](https://github.com/nisrinfrh/google_project/assets/157531427/260c80c0-d095-4fb6-848f-e52a115660b4)

### Summary of Findings

In the exploration,The analysis indicates that


The bike share service is also quite popular with the users as it has 68% of them as subscribers.
Subscribers use Cyclistic more on weekends and  mostly start their rides from 06:00 AM TO 09:00 Am and from 03:00 Pm  TO 05:00 Pm  which could indicate they use it to go to work in the morning and back home in the evening  , while for Casual
The day with the most rides is Saturday and Sunday  rider ,and mostly start their rides after 12:00pm and after 07:00pm untill 09:00 pm .###

Most rides last an average of 11 minutes and most people don't go beyond 13 minutes.The longest ride is 1409 minutes which is about 23 hours

 . cll station are the most used station by Cyclistic riders.


The mean for customers is 1.67 km, and the mean for subscribers is 1.46 km.


Key Insights for Presentation
For the presentation, I focus on the usage of the service by users according to their user category . Istart by introducing a new column called start_hour that extracts the hour of the day when the users use the service. This is an important insight because it could help the service providers know what time of day to do repairs or maintenance for their bikes with affecting their users negatively. plotted it on a *Line  chart*  to visulize most popular hour of the :-

![Screenshot (141)](https://github.com/nisrinfrh/google_project/assets/157531427/1b3bfdb6-474e-43d9-a79f-49cf72dc167c)


###Then i followed by plotting a *pie chart* showing the Ride type distribution of the users:- 

![Screenshot (142)](https://github.com/nisrinfrh/google_project/assets/157531427/d8bb1045-2516-4593-a1e3-b6bad625cdee)


###Afterwards, I looked at how each category of users uses the service per day of the week and plotted it on a *Clustered  bar chart* which showed clearly the most popular days. 

![Screenshot (143)](https://github.com/nisrinfrh/google_project/assets/157531427/aa57b87f-169b-417a-8058-c92ea3baf545)


You can view more insights by downloading and opening this file in your browse
Project Overview

This data analysis project aims to provide insights into the sales performance of an e-commerce company over the past year. By analyzing various aspects of the sales data, we seek to identify trends, make data-driven recommendations, and gain a deeper understanding of the company's performance.

bar plot






This analysis is mainly to solve the first question, How do annual members and casual riders use Cyclistic bikes differently. Based on this, i will produce a report with the following deliverable.

A. A clear statement of the business task

B. A description of all data sources used

C. Documentation of any cleaning or manipulation of data

D. A summary of the analysis

E. Supporting visualizations and key findings

F. My top three recommendations based on the analysis
Step 2: Prepare
B. A description of all data sources used.
Where is the data located? The data is located and stored in Amazon web server and is owned (first-party) by Cyclistic.

How is the data organized? Data is kept in csv with 13 columns and 5.5M rows combined (for year 2021). start coordinates are complete but the end coordinates has quite a few NULL values. The data needs to be geo-spacitally mapped to round-off the area which inturn gives the station name even if not available.

Are there issues with bias or credibility in this data? Does your data ROCCC? The data seems to fit the definition of ROCCC. Let us elaborate:

Reliable -Yes, the data is reliable as it is directly downloaded from the company’s servers. The data is a collection of all years from 2013 to 2022, for our analysis we have chosen the most recent and complete data which is 2021.

Original -Yes, the data is collected and owned by Cyclistic.

Comprehensive -The data as stated earlier is a collection from 2013 till present. We have enough data to work with given the huge historical data.

Current - The data is regularly updated by the geotrackers in the bikes. So the data satisfies this property.

Cited -no citing needed as the data is collected and owned by the companyCyclistic itself.

How are you addressing licensing, privacy, security, and accessibility? The Raw data is downloaded and kept in my laptop and will not be shared by any means and processed data will only be displayed as tables, tibbles and visualization.

How did you verify the data’s integrity? The identification of missing values ( start/end station names and their ID’s) are all identifiable given the coordinates which can be rounded off the station’s name and ID can be recovered.

How does it help you answer your question?The data provided can help me answer the underlying question earlier stated “How do annual members and casual riders use Cyclistic bikes differently?” using the following metrics of most used ride, usage behavior and most used stations for start and stop.

Are there any problems with the data?Data for around 500k/5.5M transactions is missing(start/end station name, Id’s), the challenge for me as an analyst will be either complete this data or consider the data which is complete. Considering the huge size of the data, i will be making analysis from the data available informing the stakeholders about the same to maintain transparency.

Step 3 & 4: Process & Analyse
Following are the steps in cleaning and manipulating the data

Firstly, we will use excel to clean and transform the data.So, these were the steps used: + Join the data to make one data frame + save it in a separate spreadsheet. + add two columns (i.e. ride_length and week_day) and calculate its values. + add filters to the headers and filter end_lat with empty cells. Select all the visible cells and delete them. + delete rows with negative values in ride length. + find answers to the following values using formulas in excel. Here are the results.

mode_weekday 7
mean_ride_length 00:15:37
max_ride_length 23:47:38
members_average_ride_length 00:13:21
casual_average_ride_length 00:25:04

no_of_rides_on_Sunday 17078
no_of_rides_on_Monday 17757 no_of_rides_on_Tuesday 19154 no_of_rides_on_Wednesday 20987 no_of_rides_on_Thursday 21354 no_of_rides_on_Friday 23519 no_of_rides_on_Saturday 26289

most_rides_week 26289 Saturday least_rides_week 17078 Sunday

Start loading the file in R studio for further visualization and analysis.
Key takeaways
Average ride length by customer type and day of the week: Length of the rides of Causal riders is 40% more than that of the Members.

Biketype used by each type of subcribers and casual riders Clasic bikes are No#1 in demand and electric bikes. Demand for docked bikes is very insignificant compared to the two.
####draaaaffft 

To measure the distance coverd by the users, I created a column for distance in kilometers, based on the longitude and latitude start and end points.It was clear from the distance covered by the users that most of them could only manage an average of 1.5km. The longest distance covered was 63km.

Total rides analysis by weekday Causal riders use the service for leisure and members use it to mainly commute.
