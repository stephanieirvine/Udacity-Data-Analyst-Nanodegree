# Ford GoBike Data Exploration
## by Stephanie Irvine


## Dataset

The Ford Go Bike data is from the year 2018 and, after cleaning, consisted of 1,725,137 rows with 15 features (duration_sec, start_time, end_time, start_station_id, start_station_name, start_station_latitude, start_station_longitude, end_station_id, end_station_name, end_station_latitude, end_station_longitude, bike_id, user_type, member_birth_year, member_gender, bike_share_for_all_trip). The variables are a mixture of datetimes, integers, floats, strings and categories. The categories for user_type are “Subscriber” = Member or “Customer” = Casual. The categories for gender are Female, Male or Other. A bike_share_for_all_trip variable indicates whether the rider is part of the Bike Share For All program available for those on a low income. Additional features were created including; age, month, start_hour, day of week, distance, and duration in minutes. The data was cleaned by removing null values, changing data types and also removing outliers in the member_birth_year column, therefore the data consists of cyclists from the ages of 18-65.


## Summary of Findings

In the exploration, I found that most bike trips lasted under 30 minutes with the average lasting around approximately 9 minutes. It was also found that most trips were under 2km. I found that most users of Ford GoBikes used the bikes between typical commuting hours and on weekdays suggesting that a number of cyclists were using the bikes to travel to work. Additionally, it was found that frequency would increase during the warmer months of the year and would be less during the colder winter months. 

It was found that most users of the service are subscribers compared to a rather small proportion who were customers, although it was interesting to find that when customers do use the bikes then they take longer bike trips than subscribers do on average. 

When considering how demographics affects bike trip frequency and duration it was found that the service was most popular with those in their mid twenties to mid thirties and number of users decreased after the age of thirty for every increase in year of age. Additionally it was found that males were more likely to use the service however it was interesting that when females or those who selected 'other' as their gender took bike trips then these lasted longer than those taken by males. In addition it was found that the majority of bike trips were not part of the Bike Share for All Scheme.  

When conducting a bivariate exploration of the data, it was clear there were not strong correlations between the numeric variables in the dataset i.e age, duration, distance. However, several insights into the relationships with categorical variables were found. As aforementioned, females and those identified as 'other' took longer bike trips than males and customers took longer trips than subscribers. There was no strong relationship found between duration of trip and if a participant was involved in the bike share for all scheme. It was found that the month of the year didn't have a strong effect on the duration of the bike trip, however the day of the week was related with longer trips happening during the weekends. Time of day also affected the length of the trip with longer trips during the afternoon. 

When conducting the univariate exploration it was confirmed that most bike trips were taken during the week between the most popular commuting hours. Additionally it was found that longer bike trips occurred during the weekend on average and it was surprising to find that during the weekdays the longest bike trips occurred from 1am - 3am. 


Outside of the main variables of interest it was found that females and those who selected 'other' as their gender travelled a greater distance, as did customers as opposed to subscribers, and those not involved in the bike share for all also travelled a greater distance. From the above it is clear that month or day of the week doesn't affect distance travelled however it is evident that a greater distance was travelled in the mornings, especially from 7am-8am. When investigating age most members were in their early 30s regardless of gender or user type. Interestingly, those involved in the bike share for all scheme are on average younger than those who aren't involved which is possibly as it is for low income members and it's possible these are younger on average. Younger people took bike trips at the weekend. Trips taken during very late at night and into the hours of the very early morning were taken by younger people on average.


## Key Insights for Presentation

For the presentation, I focus on the features of interest which are bike trip duration and frequency and go through the most important features to support the investigation moving from univariate, bivariate and then multivariate visualisations. I leave out duration_sec, start and end times, start and end station names and ids, longitude and latitudes and distance, bike ids and bike share for all entirely. I start by introducing the trip duration in minutes variable and plot the transformed distribution. 

Afterwards, I introduce each of the aspects of time variables in increasing order beginning with hour, day and then month. I then cover the demographic variables such as age, gender, and user type and explore the effect of these variables on frequency and then on duration of trip. When moving on to the multivariate exploration I show the heatmap of the bike trip frequency by day of the week and hour of the day. I then show the heatmap visualisation of bike trip duration by day of the week and hour of the day. I've made sure to change the colour for the last heatmap to emphasise that they are different plots. 


## Resources

https://knowledge.udacity.com/questions/205686
https://stackoverflow.com/questions/20490274/how-to-reset-index-in-a-pandas-dataframe
https://towardsdatascience.com/ways-to-detect-and-remove-the-outliers-404d16608dba
https://medium.com/analytics-vidhya/outlier-treatment-9bbe87384d02
https://stackoverflow.com/questions/26105804/extract-month-from-date-in-python/26105855
https://stackoverflow.com/questions/51102615/get-month-from-date-column
https://stackoverflow.com/questions/25754405/how-to-extract-hours-and-minutes-from-a-datetime-datetime-object https://stackoverflow.com/questions/29545704/fast-haversine-approximation-python-pandas
https://stackoverflow.com/questions/26540035/rotate-label-text-in-seaborn-factorplot
https://dfrieds.com/data-visualizations/when-use-heatmaps.html
https://matplotlib.org/3.3.1/tutorials/colors/colormaps.html 