# WeGo Public Transit

[WeGo Public Transit](https://www.wegotransit.com/) is a public transit system serving the Greater Nashville and Davidson County area. WeGo provides local and regional bus routes, the WeGo Star train service connecting Lebanon to downtown Nashville, along with several other transit services.

In this project, your goal will be to analyze data from WeGo's bus routes and attempt to identify intersections and other locations which experience frequent delays. This analysis can look by route, by direction of travel, and by day or day of the week. You can also consider time of day in your investigation (for example, comparing the AM and PM rush on Monday through Friday).

Identify Core MVP's
- identify intersections and other locations which experience frequent delays
- direction of travel affected
- day of the week impacted(7 days)
- time of day impacted(rush hour)

MVP's- What we currently are going to have trouble answering:
- Intersections: The current table does not have the functionality to map out the intersection, is there an option for that on Nashville.gov?
- What was Dan looking at in power BI? Routes with heat coloring applied to show congested areas..I feel like that may not be a resource that we have access to.
- Do we have the table with direction of travel?

Find areas of clarification for class(data definitions, data cleaning)
- will we be looking longer than a week? (month/ year analysis needed?)
- Finding averages, when and what period of time are we using?(year, month to compare days of the week.)
- What window of time will constitute rush hour for am and pm?
- What week do we want to isolate to look at routes? summer vs school year (trends between the routes)
- What constitutes a bus being 'delayed' or 'late'?
- Identify areas of needed data cleaning. (outliers? How are we identifying that?)

Potential Add options
Weather or holidays verses an average
What holiday is the most impactful to the routes running on time
How many routes were affected?


MVP's- What we currently are going to have trouble answering:
-Intersections: The current table does not have the functionality to map out the intersection, is there an option for that on Nashville.gov?
-What was he looking at in power BI? I feel like that is nota  resource that we have access to?
-Do we have the table with direction of travel?

From the current data, can not see the intersections in between stops that may be holding up traffic

You can obtain the data for this project through Swiftly. You will be provided with an API key to  access this data. The API that you will be using is the [Speed Map API](https://swiftly-inc.stoplight.io/docs/standalone/573bc3fb95867-speed-map), which provides average speed information for a single route and direction over a given date range. Note that the API can return either speed data at the stop segment level or return high resolution data, which provides information for stop segments of approximately 25 meters along with more detailed speed and duration information. Please take the time to carefully read the API documentation so that you are familiar with the query parameter options and understand the response data.

You can get more information about these routes, such as route numbers and stop information, using the [Agency Routes API](https://swiftly-inc.stoplight.io/docs/standalone/5c0bd000bb0f2-agency-routes). A user-friendly map showing all routes is available at https://www.wegotransit.com/ride/maps-schedules/bus/.

If time allows, investigate all routes, but start with the high ridership and frequent routes:
* 3: West End
* 7: Hillsboro
* 22: Bordeaux
* 23: Dickerson Pike
* 50: Charlotte Pike
* 52: Nolensville Pike
* 55: Murfreesboro Pike
* 56: Gallatin Pike

Bottlenecks - constant/irregular
*ignoring bus stop sections
Finding downtown vs suburbs bottlenecks
1st Quartile of each route for constant
*Delayed data

Focus on Inbound/Outbound

Time categories -
6am - 9am AM Peak
9am-230pm Off Peak
230pm-6pm PM Peak
6pm-6am Overnight
Day of Interest
Saturday
Sunday
Holidays*
M/F
Tues-Thurs
5/25-7/26
1/25-5/24

first Quartile
count of segments that fall into that
