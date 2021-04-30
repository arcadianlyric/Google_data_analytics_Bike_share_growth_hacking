## Google analytics certificate capstone project  

#### Background
You are a junior data analyst working in the marketing analyst team at Cyclistic, a bike-share company in Chicago. The director of
marketing believes the company’s future success depends on maximizing the number of annual memberships. Therefore, your
team wants to understand how casual riders and annual members use Cyclistic bikes dierently. From these insights, your team
will design a new marketing strategy to convert casual riders into annual members. But first, Cyclistic executives must approve
your recommendations, so they must be backed up with compelling data insights and professional data visualizations. (see pdf file for more details)  

Three questions will guide the future marketing program:
1. **How do annual members and casual riders use Cyclistic bikes dierently?**   
2. Why would casual riders buy Cyclistic annual memberships?  
3. How can Cyclistic use digital media to influence casual riders to become members?  

#### Goals
You will produce a report to answer the first question, with the following deliverables:
1. A clear statement of the business task  
2. A description of all data sources used  
3. Documentation of any cleaning or manipulation of data  
4. A summary of your analysis  
5. Supporting visualizations and key findings  
6. Your top three recommendations based on your analysis  

#### Ask
1. A clear statement of the business task \
Study the behavior difference between members and casual riders using historical data, identify trands and patterns that can help convert casual riders to members and guide digital media ads deliver.  

#### Prepare
2. A description of all data sources used \
Data downloaded from a [public source](https://divvy-tripdata.s3.amazonaws.com/index.html). I used data dated from 042020 to 032021 to reflect the most recent trends. Although the incident of COVID-19 has dramatically changed people's travel behavior, it is still useful to investigate data of the past 12 months rather than data from a normal year like 2019, because the post-pandemic influence will last for a long time and could permanently alter the travel habit. They are historical data with information on: 'ride_id', 'rideable_type', 'started_at', 'ended_at', 'start_station_name', 'start_station_id', 'end_station_name', 'end_station_id', 'start_lat', 'start_lng', 'end_lat', 'end_lng', 'member_casual', 'time_length'.  

#### Process
3. Documentation of any cleaning or manipulation of data \
Followed the standared data cleaning process (details see bike_share_report.ipynb): \
Removed missing values \
Removed outliers  
Created new metrics (riding time length, distance, time types of the day etc.)  

#### Analyze
4. A summary of your analysis \
Scripts in bike_share_report.ipynb, following PEP8 coding standards. \
Grouped ride cases by member/ casual to compare difference on time and spacial levels: \
Time: hour of day, day of week, week of year \
Spacial: most commonly used stations \
Riding time, distance, speed  

#### Share
5. Supporting visualizations and key findings \
key findings:  
1/ Station usage by member and casual rides vary. Stations popular among casual rides include many recreative palces, such as Streeter Dr & Grand Ave (close to the Navy pier), Millennium Park, Shedd Aquarium etc. 
![img](img/station_usage_compare.png)

2/ Casual rides take longer time, longer speed.  
3/ On weekend there are more casual rides and less member rides. Most rides start on Noon and Evening.    
![img](img/time_length_time_type.pdf)
![img](img/time_length_weekday.pdf)
![img](img/time_length_weekofyear.pdf)

#### Act
6. Your top three recommendations based on your analysis  
The time profile of casual riders show that they are for recreative purpose, could be tourists. If most are from other sates, they are unlikely to be converted to members.  
1/  The time
2/  
3/  

#### Act Next
Additional data needed to answer others questions  
2. Why would casual riders buy Cyclistic annual memberships?   
Need credit card or other indentity information to identify purchase made by same users and investigate conversion rate from casual to member.  
3. How can Cyclistic use digital media to influence casual riders to become members?  
Consider to deliver digital media ads near stations where most users converted from casual to member. Some A/B test will help to evaluate potential ads performance. A/B test design see **ab_test.pdf**.  

#### Appendix
scripts used for analysis in Jupyter notebook, bike_share_report.ipynb  

