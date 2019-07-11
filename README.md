# Ford-GoBike-System-Data Exploration
## by (Arushi Chawla)

## Dataset

> We are using Bay Wheels's trip data that is available for public use and is provided according to the Bay Wheels License Agreement. The dataset provides each trip's anonymized data and includes the trip, location, and user details.
The dataset is available to download from https://s3.amazonaws.com/fordgobike-data/index.html

Files were downloaded using 'requests' api which after unzipping and reading were all merged into a single dataframe. Basic data cleaning steps were performed like fixing the data types, adding new fields, removing the once not required etc.

The dataset provides each trip's anonymized data and include fields like: <br>
Trip Duration (seconds) <br>
Start Time and Date <br>
End Time and Date <br>
Start Station ID <br>
Start Station Name <br>
Start Station Latitude <br>
Start Station Longitude <br>
End Station ID <br>
End Station Name <br>
End Station Latitude <br>
End Station Longitude <br>
Bike ID <br>
User Type (Subscriber or Customer – “Subscriber” = Member or “Customer” = Casual) <br>
Member Year of Birth <br>
Member Gender <br>

## Summary of Findings and Key Insights

> As part of the analyses, we found that most of the trips were taken during the weekdays through out the month and were at peak duing the mornings 8am and evenings 5pm. We also observed that the trips were dropped during summer (May-June) and winter (Nov-Dec) weathers. A drop in the trips were also seen around 11/2018 which were agin picked up after 01/2019. <br>
Further interesting observations were the males having ~67% higher trips than females and the age group 20-40 having 68% of the total trips. <br>
There were top 3 stations spotted which had way too many trips when compared to others pointing us in a direction that these stations are most frequently visited. The comparison between subscribers and customers showed subscribers having 82% of the trips which could be related back to high trips on weekdays 8 am and 5 pm and to same stations. An hypothesis could be generated here that most of the subscribers take daily trips to the work or schools. Moreover, the avg. trip duration for 75% of the trips were within 15 mins which could mean subscribers either live close by to their destinations or drive to the start station for a shorter trip. The avg. duration for customers however, was quite higher and esecially from 1am to 4am we could observe 25-35 min trip which could mean they mostly are exploring the bikes and/or are one-time riders.

