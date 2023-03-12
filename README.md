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
* The homepage serves as an introduction to the project, providing a concise overview of its purpose and contents. 
<img width="1022" alt="Screenshot 2023-03-11 at 11 23 10 PM" src="https://user-images.githubusercontent.com/115101031/224524288-b3f378bf-a72a-4292-b7eb-a7a3820c2c0e.png">

### Ride Analysis 
<img width="1001" alt="Screenshot 2023-03-11 at 11 23 25 PM" src="https://user-images.githubusercontent.com/115101031/224524307-5c4c58f0-f726-4c3a-b2f5-8bc9b657fafc.png">

### User Analysis
<img width="999" alt="Screenshot 2023-03-11 at 11 23 53 PM" src="https://user-images.githubusercontent.com/115101031/224524319-c66f9bb1-e78c-45b7-9c03-043a61b9d9b8.png">

### Trip Analysis
<img width="1002" alt="Screenshot 2023-03-11 at 11 24 07 PM" src="https://user-images.githubusercontent.com/115101031/224524331-2433f520-8d19-48b7-aaab-f7c56778033c.png">

### Geographic Analysis
<img width="1004" alt="Screenshot 2023-03-11 at 11 24 27 PM" src="https://user-images.githubusercontent.com/115101031/224524338-25be803d-a9fd-41fc-9148-45bf8646c9c3.png">
<img width="1000" alt="Screenshot 2023-03-11 at 11 24 45 PM" src="https://user-images.githubusercontent.com/115101031/224524388-23e95637-7d20-49fc-9525-e88c9613c276.png">


## Summary

### Ridership Analysis
* Ridership was higher in the same time period in 2023 by both those holding memberships and by casual users.
* January 2023 showed a significant increase in use by members over 2022.
* Ridership was generally up every weekday in the time period under review for 2023.  In general, Sunday's and Monday's saw a significant increase in rides in 2023, as compared to the same time period in 2022.
* Rides taken between 11am-6pm representated the highest volume of riders using the program.

### User Analysis
* 6th and 7th Avenue and Central Park are among the most popular start and end stations among users.  
* Locations around Central Park seemed to monopolize the top 10 stations overall.
* Both Citi Bike members and casual users seemed to prefer classic bikes, but casual users showed a higher frequency of selecting electrical and docked bikes.
* After creating a new calculated measure to determine trip duration between start and end stations for all recorded rides, as expected, casual users of the program showed the greates variance in recorded trips.

### Trip Analysis
* Classic bikes are among the most used in the program.
* Docked bikes experienced a decrease in duration of trips between 2022 and 2023 for the same time period., while electric bokes increased in the same timeframe.

### Geolocation Analysis
* A close-up geographical view of the top 50 stations, shows a high level concentration around popular sites in New York City, including Central Park and 5th and 6th Avenue, popular for dining, shopping, and cultural attractions.  Additional stations in our top 50 focus around midtown Manhattan and Union Square,  These focal points seem consistent between the same time period in 2022 and 2023.
* Trip duration between start and end stations also seem consistent with these geographical focal points. 
* The second set of maps are scaled to trip duration and show a consistent distribution for members,with a few stations on the edge of the city showing the longest trips.  Casual users tend to show the longest trips around high traffic areas of the city, often those frequented by tourists.

### Overall conclusions
* Despite raising prices for use of the program in January 2023 (prices also increased in January 2022), and poor reviews, ridership has increased.  With a mission to increase bikeshare ridership and transportation, several campaigns and initiatives over the 2022/2023 year seem to have paid off.
* Members show the least amount of variance when using the program.  As regular users, trip duration for members tends to fall close to the mean.  Casual users, on the iother hand, show a greater degree of variance from the mean.  This is likely because casula users may account for visitors to New York City, and therefore, their use will depend on a planned excursion or destination.
* Between 2022 and 2023, Citi Biek increased the number of electrical bikes in the program.  These seem to be more concentrated in areas of hgh traffic (ie. tourist locations) and thus more likley to be used by casual riders than members.
* Geographical analysis of the top 50 stations indicates effective placement of bike stations.  The most popular member bike locations and trip duration focuses on neighbourhoods, showing that use provides effective and convenient options for members to go about their daily activities.    For casual users, the most frequented stations congregate around high traffic areas, such as top tourist destinations for the city.  Stations indicating the longest trips tend to also focus around some of the most popular destinations in the city.

By transforming the data actively collected by Citi Bike officials into a dashboard, I am able to tell a story that demonstrates:
1) That there are clear patterns defined by the data, in terms of use of the program and the users of the program.
2) Citi Bike officals can use this data to make decisions about locations/stations that might not be as frequently used, and thus allocate their resources in more effective locations, maximizing convenience for users, and profititability for the program as it grows.  





