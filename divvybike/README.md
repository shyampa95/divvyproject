# Final Project

Team Members :- Shyam Patel

### Data

We are re-examining the Divvy bike data we initially used in our ETL project for our final project.. See 

https://www.divvybikes.com/system-data for the original csv files.
<br>
<br>
<br>
### Tableau

Before diving headfirst into our machine learning section, we discovered that Tableau was a great tool for experimenting with the data and looking for intriguing trends.. Here are some of the things we found.

###  Age Distribution of Divvy Rider Base

- The overall average age of Divvy riders is 36 years.
![alt text](https://github.com/shyampa95/divvy_bike_final_project/blob/master/charts/Age_distribution.PNG)

### Trip Durations by Gender  
- The overall average trip duration is 24.39 minutes.
- Keep in mind that this includes "null" values - Divvy only collects demographic information for members, so there is a large portion of data that does not include gender information.
- There's not a big difference between male and female trip duration (but we can infer here that non-members seem to take longer trips than members do - this might be something interesting to look into if we wanted to spend more time on this!)

![alt text](https://github.com/shyampa95/divvy_bike_final_project/blob/master/charts/Trip_duration_vs_gender_including_nulls.PNG)

### Most Popular Stations  
- Top Departure Station: Streeter Dr & Grand Ave (21,741)
- Top Destination Station: Canal St & Adams St (17,198)
- We created a Leaflet map that shows the location of these stations, and shaded by census tract to help us visualize the Chicago neighborhoods

![alt text](https://github.com/shyampa95/divvy_bike_final_project/blob/master/charts/Top_20_Departures.PNG)
![alt text](https://github.com/shyampa95/divvy_bike_final_project/blob/master/charts/Top_20_Destinations.PNG)
![alt text](https://github.com/shyampa95/divvy_bike_final_project/blob/master/charts/map_example.PNG)

<br>
<br>
<br>

### The Website
We used bootstrap and some HTML/CSS magic to create a website to display these visualizations, featuring:
- An analysis section including link to our graphs
- An interactive section with a tabular menu option. The user can switch between "Traffic" and "Map"
- A link to our github (you are here!)

![alt text](https://github.com/shyampa95/divvy_bike_final_project/blob/master/charts/Website_view_1.PNG)

<br>
<br>
<br>

### Machine Learning

### Linear Regression Models

- We found that a simple, single-layer machine learning model with a linear regression (or anything else) wasn't smart enough to determine any real trends in the data. However, we were able to validate a couple items that did not correlate, which is occasionally just as fascinating..

- For example, see the plot below - it corroborates the bar graph we got from Tableau, showing that there's not much of a difference between the male and female riders when considering trip duration, however, the "null" gender group is skewed a bit toward the high side.

![alt text](https://github.com/shyampa95/divvy_bike_final_project/blob/master/charts/GenderVSduration.png)

### Random Forest

- Next, we moved on to a random forest model, which required running on Zepl because our poor tiny local machines crashed when we tried a Jupyter notebook..


### Neural Networks

Hence, we employed a neural network! This provided us with more insightful information and helped us go far further than our initial Tableau explorations could.
