# (FordGoBike Dataset Exploration)
## by (Jerome Gameli Kofi Davor)

## Introduction
In this project I analyze information that covers over 180K records of individual rides made in a bike-sharing system covering the greater San Francisco Bay area.

This notebook is mainly aimed to get an overview of the dataset and answer important questions regarding bike trips (No., time, users, .....etc) which will be shown along the notebook via exploratory & explanatory data analysis & visualizations.

Coding will be via python's different libraries for data analysis (Pandas, Matplotlib, Seaborn) for data wrangling, cleaning and creating storytelling visualizations.

## Dataset

This data set contains information from the FordGoBike System about individual rides made in a bike-sharing system covering the greater San Francisco Bay area. 

The dataset has quality and tidyness issues and theses will be addressed after the preliminary data wrangling stage.

The dataset contains:

* An id for each bicycle
* The trip duration in seconds
* Start time for the trip
* End time for the trip
* The id of the station where the trip started
* The name of the station where the trip started
* The latatitude of the start station
* The longitude of the start station
* The id of the station where the trip ended
* The name of the station where the trip ended
* The latatitude of the end station
* The longitude of the end station
* The users of the GoFord bike service (classified into customers and subscribers)
* The users' birth year
* The users' gender (classified into male, female and others)

Feature Engineering of dataset: This was carried out to further derive valuable information from the orignal dataset. They include:

* Trip duration in minutes
* Trip duration in hours
* From users' birth year, users' age were determined
* Month the trip took place
* Days of the week
* Distance travelled in kilometer
* Speed in km/hr
* Age group (classified into young adults, middle aged adults, seniors)

There were some cleaning needed in the dataset as earlier mention.

* Empty columns in bike_df dataframe.
* Wrong data types.
* Time is recorded in seconds
* There were some redundant columns in the dataset.



## Summary of Findings

> Summarize all of your findings from your exploration here, whether you plan on bringing them into your explanatory presentation or not.

* After cleaning the dataset, it is discovered that 91% of the user types are subcribers, and only 9% are customers.

* The mean age is found to be 33.1 years old, and after cleaning the data, the oldest age is 79 years old, and the youngest is 17 years old.

* The majority of the riders are males, making up 75% of the ride sharing population. 23% are females while 2% identify as other.

* Service usage by days of the week: Customers showed consistency across the week while subscribers rode mostly during the weekdays with a sharp decline on weekends. Both user groups shared the same peak day (Thursday). It also showed that customers are more likely to use the service during weekends unlike subscribers. Same applies to gender role on days of the week.

* User type vs Distance : Customers have a higher average distance travelled than subscribers.

* Speed and Distance: Subscribers record a lower distance with a higher speed while customers travel higher distance at a lower speed.

* Age group vs speed: Generally one would expect that as age increases, average speed reduces (this was visibly shown in bivariate exploration).

* Creating age group classification: This made it visually easy to see how speed and distance varies by age group. As age reduces distance and speed increases, and vice versa. It also shows the dataset is mostly made up of young adults, meaning younger people used the service (customers or subscribers) the most for the month of Feburary.


## Key Insights for Presentation

> Select one or two main threads from your exploration to polish up for your presentation. Note any changes in design from your exploration step here.

* The 1st key insight for presentation is the service usage difference between customers and subscribers.

* The 2nd key insight for presentation, user type vs distance. How does age group affect users distance covered. Determining if a specific age group is contributing to the distance covered by users.

* The 3rd key insight for presentation provides more information on how distance, speed and age groups are related.
