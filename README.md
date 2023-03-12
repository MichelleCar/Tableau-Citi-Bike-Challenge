# Citi Bike Analysis with Tableau
![images](https://user-images.githubusercontent.com/115101031/224523484-c6ea3ce2-7ad7-4e0b-a21b-fafa99a3a802.jpeg)

## Background 
Since 2013, the Citi Bike program has implemented a robust infrastructure for collecting data on the program's utilization. Each month, bike data is collected, organized, and made public on the [Citi Bike Data](https://citibikenyc.com/system-data) webpage.

However, while the data has been regularly updated, the team has yet to implement a dashboard or sophisticated reporting process. City officials have questions about the program, so your first task on the job is to build a set of data reports to provide the answers.

## Deployment
Please find below the link to the Tableau dashboard, showcasing the results of the analysis: https://public.tableau.com/views/CitibikeChallenge_16785020317790/CitiBikeAnalysis?:language=en-US&:display_count=n&:origin=viz_share_link

## Methodology
My task, as the data analyst, is to build a set of data reports to address their questions about the program.  In looking for an effective avenue of inquiry, I used 4 data sets: January and February for 2022 and 2023.

Questions I am hoping to answer for city officials:
1) Is there a discernable pattern of use of the program over a similar time period from 2022 to 2023?
2) How can certain patterns of use inform city officials on ways to improve the program.

## Data Source
Using data from the Citi Bike site (https://citibikenyc.com/system-data), the focus of my analysis is the comparison of the first two months of 2023 with the first two months of 2022.

The data sets required some cleaning, including merging the data sets into one DataFrame, converting data into proper date/time format, creating a column to hold trip duration for each trip for the purpose of excluding any trip less than 30 minutes.  Finally, I removed any rows with null values in any column, and exported the final filtered and clearned DataFrame to a CSV file.

<img width="690" alt="Screenshot 2023-03-11 at 11 14 53 PM" src="https://user-images.githubusercontent.com/115101031/224524090-b2e2d67e-15da-41ac-a10a-798a80085e29.png">
<img width="608" alt="Screenshot 2023-03-11 at 11 16 45 PM" src="https://user-images.githubusercontent.com/115101031/224524102-3a4937e6-65e9-4820-a98a-18d76365ac04.png">
<img width="594" alt="Screenshot 2023-03-11 at 11 16 55 PM" src="https://user-images.githubusercontent.com/115101031/224524109-a786ebf6-2ead-4834-8763-b92d7eaa6285.png">
<img width="585" alt="Screenshot 2023-03-11 at 11 17 07 PM" src="https://user-images.githubusercontent.com/115101031/224524115-9f674fca-8f21-4340-8a8c-f306758209f6.png">
<img width="587" alt="Screenshot 2023-03-11 at 11 17 16 PM" src="https://user-images.githubusercontent.com/115101031/224524124-aa863ae8-89b8-403c-aa9e-40a3fb4b0f2f.png">
<img width="587" alt="Screenshot 2023-03-11 at 11 17 26 PM" src="https://user-images.githubusercontent.com/115101031/224524133-dcacc0d6-dc7e-4230-a51c-21c8b27bd506.png">
<img width="586" alt="Screenshot 2023-03-11 at 11 17 34 PM" src="https://user-images.githubusercontent.com/115101031/224524145-d1e777e4-5e71-4d8d-809d-4d8224afdd3b.png">

## Dashboards
Looking at the most recent data available (January and February 2023), I wondered if meangingful analysis and conclusions could be drawn by  comparing it to the 2022 data sets for the same two months.  For example:
1) Total ridership (bar chart)
2) Ridership by weekeday (treemap)
3) Ridership  by time of day (heat map)
4) Bike preference by users (pie chart)
5) Comparison of trip duration between Citi Bike members versus casual users (customised shape chart)
6) Trips by bike type (bubble chart)
7) Average trip duration by bike type (bar chart)
8) Top 10 start and end stations (scaled bar chart)
9) Geolocation of top 50 start and end stations (map, with toggles for year)
10) Average trip duration for the top 50 start and end stations (map, with toggles for year)

### Homepage
* The homepage serves as an introduction to the project, providing a concise overview of its purpose and contents. It clearly summarizes the key insights and findings of each dashboard, allowing for quick and easy navigation.
<img width="1425" alt="Screenshot 2023-02-13 at 8 21 56 PM" src="https://user-images.githubusercontent.com/112406455/218622889-c2c2e218-99cc-4f3f-989b-e50da7169004.png">

### User Analysis 
* The dashboard presents a comprehensive analysis of the Citi Bike trips, taking into account various factors such as user type, gender, and age. Additionally, it provides an in-depth examination of trip patterns based on the hour of day and day of the week, as well as the total number of trips per month.
<img width="1426" alt="Screenshot 2023-02-13 at 5 32 45 PM" src="https://user-images.githubusercontent.com/112406455/218599192-abf1dfc0-9a14-4d48-8a7a-683cdbf34528.png">

### Station Analysis
* The dashboard focuses on the analysis of trips in relation to the bike stations. It compares the trip patterns between weekdays and weekends and provides insights into the average trip duration for each month.
<img width="1424" alt="Screenshot 2023-02-13 at 8 22 32 PM" src="https://user-images.githubusercontent.com/112406455/218623090-2424212c-a74c-4962-a0a4-8cb6698d0327.png">

### Geographic Analysis
* The third dashboard features two maps showcasing the geographical locations of the start and end stations. The size and color of the markers are used to represent the total number of trips that originated or terminated at each station, providing a visual representation of the trip patterns and frequency.
<img width="1425" alt="Screenshot 2023-02-13 at 5 33 31 PM" src="https://user-images.githubusercontent.com/112406455/218600539-d287fd71-6f8b-4e2d-805a-e60477abd38b.png">

**A user-friendly interface has been created utilizing Tableau dashboards, allowing for seamless navigation between pages. Please access the link in the deployment section to explore the interactive dashboard and gain valuable insights.**

## Summary
<img width="986" alt="Screenshot 2023-02-13 at 6 17 04 PM" src="https://user-images.githubusercontent.com/112406455/218605560-74bbe56a-b822-4b78-b39e-956f143bfffa.png">

* An evaluation of the data covering the time period from 2018 to 2020 shows a total of 1,095,641 trips made using bicycles in New York City. This represents a decrease of 4.83% over the three-year period. The observed decline in trips can be attributed to the adverse effects of the COVID-19 pandemic, including the associated shutdowns, on the usage of bicycles.
* A comparison of the data from 2018 to 2020 reveals a decrease of 30.20% in the number of subscribers, while there was a simultaneous increase of 374.90% in the number of customers. This disparity in trends can be attributed to the impact of the COVID-19 pandemic on the usage of bicycles in New York City.
* Over the specified time period, there appears to be a positive trend in the number of female riders, with an increase of 12.55%, while the number of male riders has decreased by 22.29%. While the reason for this trend is not definitively known, it could potentially be attributed to improved safety and security measures for female riders. Further analysis would be required to establish this hypothesis.

<img width="822" alt="Screenshot 2023-02-13 at 6 46 50 PM" src="https://user-images.githubusercontent.com/112406455/218609202-043e2682-5796-42c4-91c1-5bdad3f347ad.png">

* It is noteworthy that the peak utilization of citibikes in New York City occurs during the weekday, specifically during the hours of 8 a.m. and 5 p.m., as a significant number of commuters utilize bicycles for their daily commute.

<img width="589" alt="Screenshot 2023-02-13 at 6 56 45 PM" src="https://user-images.githubusercontent.com/112406455/218610532-c600a3e0-0abc-431d-bb29-5a2d90f447e7.png">

* An examination of the data reveals that the pattern of peak bicycle usage in New York City remained consistent during 2018 and 2019, with the busiest periods occurring during the weekdays. However, in 2020, a notable deviation from this trend emerged, with weekends experiencing the highest levels of bicycle usage. This shift can likely be attributed to the widespread adoption of remote work as a result of the COVID-19 pandemic. 

<img width="621" alt="Screenshot 2023-02-13 at 7 05 26 PM" src="https://user-images.githubusercontent.com/112406455/218611841-d35104a1-4fe0-4b5b-9669-f3fc596f4eb4.png">

* A review of the data by month reveals that the highest usage of bicycles in New York City occurs during the summer months of July, August, and September, in comparison to the winter months. In April of 2020, a marked decrease in bicycle usage was observed, which can be attributed to the restrictions imposed during the early stages of the COVID-19 pandemic.

<img width="602" alt="Screenshot 2023-02-13 at 7 05 30 PM" src="https://user-images.githubusercontent.com/112406455/218612417-bc985457-005a-453f-a641-3425d3a01e91.png">

* The analysis of the data indicates that the majority of bicycle riders in New York City belong to the age group of 29 to 43, with a prevalence of male riders among this demographic.

<img width="1163" alt="Screenshot 2023-02-13 at 7 19 08 PM" src="https://user-images.githubusercontent.com/112406455/218614331-c7e16678-be24-4ba5-a91e-700b3da6248a.png">

* An examination of the data reveals a disparity in the number of start stations compared to the number of end stations.

<img width="812" alt="Screenshot 2023-02-13 at 7 19 16 PM" src="https://user-images.githubusercontent.com/112406455/218614627-d3fa0863-5a3d-4b8b-ad3b-6ccdf6c28036.png">

* The analysis of the data, as depicted in the chart, indicates that Grove St PATH and Hamilton Park are the most frequently used stations for both starting and ending trips.

<img width="615" alt="Screenshot 2023-02-13 at 7 19 20 PM" src="https://user-images.githubusercontent.com/112406455/218615289-c4ec6639-0ecd-4d15-9ada-11ac052315d8.png">

* An examination of the graph presenting the average trip duration, measured in minutes, per month reveals a noteworthy increase in 2020 compared to the average trip durations in 2018 and 2019. This deviation can be attributed to the closure of businesses and an increased amount of time spent outdoors, particularly during the summer months, as a result of the COVID-19 pandemic. 

<img width="1254" alt="Screenshot 2023-02-13 at 7 46 06 PM" src="https://user-images.githubusercontent.com/112406455/218617657-e904b6a8-31b1-4f15-be80-ba9c807653b9.png">

* An analysis of the start station map highlights the concentration of the most frequently used stations in Jersey City, New Jersey, primarily in the zip codes 07302 and 07310. This suggests that the residents of Jersey City utilize the bicycle-sharing service extensively, potentially due to its cost-effectiveness when compared to other transportation options, such as taxis and ride-sharing services.

<img width="1252" alt="Screenshot 2023-02-13 at 7 46 55 PM" src="https://user-images.githubusercontent.com/112406455/218618488-3f4ff112-edab-4dfa-8e52-92d6ddc2e050.png">

* Similar to the start station map, the end station map also illustrates a notable concentration of the most frequently used stations in Jersey City, New Jersey, indicating that residents are likely utilizing the bicycle-sharing service for their commutes to and from work. 

## Conclusion
In conclusion, this Tableau analysis provides a comprehensive overview of the trends and patterns in Citibike usage over a specified time period. Through the creation of interactive dashboards and visualizations, key insights have been extracted and presented, highlighting trends in user type, gender, and age, as well as trip patterns based on hours and weekdays. One noteworthy phenomenon observed from the overall analysis is the high usage of the Citibike service by residents of Jersey City, New Jersey, primarily for commuting purposes. This analysis serves as a valuable resource for anyone interested in understanding the usage of Citibike and exploring the data behind this popular bike-sharing service. I hope that this work will inspire further research and investigation into the data, and encourage others to build upon the insights presented here.





