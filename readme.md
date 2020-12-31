# Bay wheels Trip Data Exploration

## Dataset

The data consists of information regarding trip data of Lyft ebikes in the month
of November. https://s3.amazonaws.com/baywheels-data/index.html. The dataset is 
in 201911-baywheels-tripdata.csv. There were 185496 rows and 15 columns.


## Summary of Findings
The distance was computed for each row based on the haversine formula based on
the start and end latitude and longitude. The distance follows a close linear 
relationship with the time for short periods but falls after that.
Some of the distances were zero suprisingly and for some others it was huge 
with some latitudes and longitudes marked as zero.
Many transit stations figured in the popular start and end stations.
The usage of bike share for all and clipper usage were very small.
The distance travelled and duration of the trip varied based on the user type
- whether they were a customer or a subscriber. There were higher for customers
than they were for subscribers, though the number of subscribers is far higher 
than customers.
Driving home the point, even the station usage for similar distances, were widely
different based on the user type.


## Key Insights for Presentation

For the presentation, I focus on the distribution of distance and time and their
relationship. Also, I focus on the relationship of distance and time on the user 
type. To further drive home the point, I divided the datatype into three tiers 
based on the distance. Then I found out the stations based on the mean time of
travel for the user types. There was no common ground between the two.
But it brings home the point that the customers generally bring more revenue 
because of their increased usage and should be paid just as much attention as
subscribers.
