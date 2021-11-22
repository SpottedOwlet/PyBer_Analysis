 <h2> <p align=center>PyBer Ride Sharing App Analysis</p></h2>

<h3> Background & Purpose </h3>
The rideshare data for PyBer app company has been analyzed using exploratory data analysis with the goal of improving access to ride-sharing services and to determine affordability for undeserved neighborhoods.  This report takes further account of the total weekly fares for each city type using the multiple-line graph. Let us take a closer look at the analysis, results and recommendations based on the results of the analysis in the following sections.


<h3> Resources </h3>

  - Data Source: city_data.csv, ride_data.csv
  - Software: Python 3.7.10, Jupyter Notebook

<h3> Overview Of The Analysis </h3>

<h4> Data Preparation: </h4>
<p>
In the first step, city_data and ride_data were imported into two separate dataframes. They were then checked and verified for any null values and columns were verified for the correct data types. The two dataframes were merged together to get the desired metrics for the summary dataframe.
</p>


<p align=center><kbd>
  <img width="598" alt="pyber_summary_df" src="https://user-images.githubusercontent.com/90424752/142752766-91abc1dc-0f69-4f1a-a6aa-a454771b2666.png">
</kbd></p>

<h4>Preliminary Analysis From The Ride-sharing Summary Dataframe: </h4>

The summary dataframe contains total and average metrics by ciy types. It gives us clarity on the city-wise counts of total rides, total drivers, total fares and also averages of city-wise per ride fares and per driver fares. The observations from the summary dataframe are listed below:

- The number of rides are highest in urban areas and lowest in rural areas. The numbers for rides in suburban areas lie in the middle range of that of urban and rural areas. 
- The number of drivers also follow the same pattern seen for the number of rides, going from highest to lowest from urban to rural.
- Total Fares, Average Fare Per Ride and Average Fare Per Driver, all follow the exactly opposite trend from the one observed in Total Rides and Total Drivers. All the fares go from highest to lowest from Rural to Urban areas, suburban being in the middle range. 

<h4>Conclusion:</h4>The data in the summary dataframe shows that the Fares are driven by the number of rides and drivers available in the city. Fares show negative correlation with the two variables in consideration: rides and drivers.


<h4> Total Weekly Fares Analysis For Each Type Of City: </h4>
For this analysis, a new dataframe containing city-wise fares for each date is filtered out from previously merged dataframe pyber_data_df. This dataframe is further processed to create a pivot table. The city-wise fare data from Januray 01, 2019 to April 28, 2019 is captured in a new dataframe using pandas loc function and the date column which is also an index, is set to the date-time format. In the next step, weekly_pyber_fares_df captured the weekly sums for fares for each city type.


<p align=center><kbd><img width="258" alt="weekly_fares" src="https://user-images.githubusercontent.com/90424752/142755181-2afca0c8-07dd-4ecd-8f0c-e0b50cee2f46.png"></kbd></p>

<h4> Plotting The Multiline Graph </h4>
Using the above dataframe, we are doing exploratory data analysis to understand the data, relationships between the variables and to discover patterns within the data. Graphical representation fo the data is an integral part exploratory data analysis which helps us understand the data better. The data in the above dataframe is plotted in the form of multiple line plot to gain more insights.


<kbd><img width="994" alt="Fares by City type" src="https://user-images.githubusercontent.com/90424752/142751390-1021a0f0-1109-4ffc-8b26-8616609b23c7.png"></kbd>

<h4> Observations: </h4>

- The total fares for urban and suburban areas rise during the first week of January, on the contrary rural areas show a slight decline during the same time. 
- All three areas show a dictinct rise in fares in the third week of February.


<h3> Results </h3>

- The number of rides are highest in urban areas and lowest in rural areas. The number for rides in suburban areas lie in the middle range of that of urban and rural areas. 
- The number of drivers also follow the same pattern seen for the number of rides, going from highest to lowest from urban to rural.
- Total Fares, Average Fare Per Ride and Average Fare Per Driver, all follow the exactly opposite trend from the one observed in Total Rides and Total Drivers. All the fares go from highest to lowest from Rural to Urban areas, suburban being in the middle range. 

<h3> Summary </h3>

The summary dataframe explores the relationship between rides, number of drivers and fare metrics. It brings into the limelight, that the majority of revenue is generated in the urban areas followed by suburban and lastly rural areas. It also indicates that the fares are negatively correlated with the number of rides and drivers in the areas. This is an important insight in order to strategize the business recommendations.

The multiline plot explores the trends shown by total weekly fares by each city type from January 2019 to April 2019. From the exploratory analysis carried out on the pyber data, following business recommendations can be made:


<h4> Business Recommendations </h4>

1. To increase the revenue generated by densely populated urban areas while attracting more customers following strategies could be used:
  - Usage based percentage or flat rate discounts
  - Pyber Credits to new customers
  - Increased advertising would be effective towards attracting new customers in urban areas.

2. The suburban areas could use a mix of promotional offers, advertisements and also offer some additional benefits to new drivers signing up from suburban areas.

3. The higher fares in the rural areas might act as a discouraging factor. Rural areas could use following types of promotional offers to encourage more people to use the pyber ride-share service.
  - Promotional discount offers to repeating customers
  - Pyber Credits to new customers
  - Drivers signing up from rural areas could be given extra benefits to increase number of drivers from rural areas.
  - Advertising would make more people aware of the benefits and 

The recommendations made above, should be reinforced with additional analyses suggested below :
  - The EDA (Exploratory  Data Analysis) should be performed on the data from past years to confirm the trends and patterns found in this analysis.
  - The demographics relating to this data could be studied using EDA to discover trends shown by different age groups. Findings from this analysis could be used to strategize the recommendations for urban, suburban and rural areas.




