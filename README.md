# Business-Intelligence-

## Business Task
The product development team at Cyclistic has begun developing their business plan for next year. In order to build a better Cyclistic, the team needs to understand how customers are currently using the bikes, how location and other factors impact demand, and what stations get the most traffic. These insights will inform new stations and identify customer’s demand at different station locations.

## Data used
Three data set were used, two (2) from Big query and one (1) containing Zip codes
+ `bigquery-public-data.new_york_citibike.citibike_trips`
+ `bigquery-public-data.geo_us_boundaries.zip_codes`
+ `planar-granite-404916.Cylistic.zip_codes`

## Steps
+  In preparing for this project, I clearly understood the stakeholders and team requirement and developed a comprehensive project plan document (Stakeholder, project and strategy requirement document) outlining key objectives, approaches, timelines and strategies for the analysis. The document guided the entire project process.
+ SQL queries were developed using big query console to extract data from the multiple sources in the data lake, it transformed and loaded to the target table. 
+ The target table was loaded into the tableau environment for visualizationa and to gain insight from the data.
  

## Data visualization(Tableau Dashboards) 
![BI Dashboard](https://github.com/Samfocus/Business-Intelligence-/assets/152339100/aa7b7e8b-583b-4a7f-8eff-0c495df2d894)
+  The first tab of the dashboard presents a comprehensive view of seasonal bike trip trends across New York boroughs for the Cyclistic company. This map showcases individual neighborhoods, comparing the number of trips and average trip durations for both customers and subscribers. Notably, July, August, and September emerge as peak months for bike traffic. The interactive dashboard incorporates filters for user types, metrics, months, and specific starting or ending neighborhoods. Clicking on a borough updates the table and maps, offering detailed insights. Additionally, the dashboard delves into seasonality with the Trip Totals chart and the Trip Counts by Starting Neighborhood table, providing valuable information for identifying customer demand, influencing new station placement, and optimizing traffic dynamics. Also the chart at he lower part of the dashboard for utilizes the Trip Totals chart on Tableau to visually represent the total number of bike trips taken in 2019 and 2020, distinguishing between customers and subscribers. Notably, the chart highlights that subscribers constitute a significantly larger user base for Cyclistic than regular customers. Furthermore, it illustrates a notable increase in users during warmer months (May–October) compared to colder months, aligning with the expected decrease in bike ridership during colder weather. This insightful visualization, achieved by aggregating Start Day by month in the columns field, summing Trip Counts in the rows field, and assigning UserType as color assignment, provides valuable information on user behavior patterns and seasonal variations that can inform decisions regarding new station placements and optimizing bike availability.


  
![BI Dashboard3](https://github.com/Samfocus/Business-Intelligence-/assets/152339100/712707b8-486f-49c7-a79e-2cadfcaccd35)
+  The second Tableau dashboard for Cyclistic provides a comprehensive view through the "Trip Counts by Starting Neighborhood" table, detailing the total number of bike trips initiated in each neighborhood across 2019 and 2020. The table, organized by zip code, borough, and neighborhood, employs a color gradient to visually highlight variations in monthly trip counts, with darker shades indicating higher trip volumes. To ensure readability, the table uses light text on darker values. This detailed breakdown is particularly valuable in understanding user behavior and demand, emphasizing the importance of starting locations when considering advertising and station placements. Notably, the most active stations, such as those in the Lower East Side and Chelsea and Clinton neighborhoods, are identified, and the peak activity months from May to October are highlighted. This insightful visualization, achieved by strategically placing dimensions and measures in Tableau, offers key insights to guide decisions on new station locations and advertising strategies for Cyclistic.

![BI Dashboard2](https://github.com/Samfocus/Business-Intelligence-/assets/152339100/c0d3d25d-a4de-4b1f-a453-285fa15c29c7)
+  The third and final tab of the Cyclistic dashboard presents a compelling comparison of the total number of trip minutes categorized by starting and ending neighborhoods for both customers and subscribers. Utilizing horizontal stacked bar graphs, these charts offer a visual representation ordered from the highest to lowest number of minutes, amalgamating data for both user types. The insights gleaned from these charts reveal the locations where users are most inclined to embark on longer journeys. Specifically, the Lower East Side and Chelsea and Clinton neighborhoods emerge as having the highest combined total trip minutes for both start and end stations. To create the starting neighborhood chart, one can place the sum of Trip Minutes in the columns field, with Zip Code Start, Neighborhood Start, and Borough Start dimensions in the rows field, employing UserType for color assignments. Similarly, the ending neighborhood chart is crafted by replicating these steps with Zip Code End, Neighborhood End, and Borough End dimensions. This visualization provides crucial information for Cyclistic in understanding user travel preferences and can inform decisions on station placement and marketing strategies


