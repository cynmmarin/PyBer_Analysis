# PyBer_Analysis
Module 5: PyBer with Matplotlib

## Overview of Project
### Purpose
In our analysis we will be generating a multiple-line graph to showcase the total weekly fares that PyBer drivers received on cities. Pyber is a Python based ride sharing company which marketÕs its product on Urban, Suburban and Rural cities. We will be able to determine which city type has the highest traffic and make an assessment to address the inequalities in the three city types. 
In this study we will write a Python scripts, using Pandas's libraries, Jupyter Notebook and Matplotlib to obtain the following information per city type: Total rides, total drivers, total amount of fares, average fare per ride and average fare per driver. Once this data has been gathered, we can go ahead and obtain the total fares by dates and create a chart which displays the relationship of dates and fare coast and their effect on total fares by city type. 
## Results
We will be using the two data sets, *city_data_to_load* and *ride_data_to_load* to obtain the information needed for our analyses. The raw data contains the "Type" of city, the "City", "Driver_Count", "Date", "Fare" and "Ride_ID". We will start by creating DataFrames and merging it to kickoff our evaluation. We will call the new DataFrame, "pyber_data_frame" and go ahead and get a summary of Pyber's presence and driver's revenue in Urban, Suburban and Rural cities. 

### Total Drivers for each City Type
In order to obtain the total number of drivers for each city type, we need to use the ÒgroupbyÓ function and apply it to our ÒtypeÓ data. Then, obtain the sum, using the "driver_count". Once we run this script, we find out that: The total driver for Rural cities is 78. The total drivers for Suburban cities 490. And that the total drivers for Urban cities is 2405. Therefore, the city type with the most drivers are Urban cities and the city type with the least activities are Rural cities. We can make the assumption that Pyber's service is not as enticing and suitable for Rural cities. This can be an issue with the population number, but we do not have enough data right now to make a substantial assumption. 

### Total Amount of Fares per City
The fare count per city type, is obtained using the "groupby" function and filtering through city and summing it and using the fare data to find out the total amount. Once this data is obtain, we see that the total fares for Rural cities is $4,327.93. The total fare for Suburban cities is $19,356.33. Meanwhile the total fares for Urban cities was $38,854.38. Therefore, Urban cities continue to be the city type with the highest traffic of Pyber users and therefore the most profitable for the drivers. It seems unlikely for a driver to want to relocate to a Rural city to work, if they can have access to a larger pool profits. 

### Average Fare per City and Average Fare per Driver
The average fare per city is computed by dividing the "total_fares" by the "total_drivers", this gives us the following information: The average fare for Urban cities is $24.52, for Suburban is $30,.97 and for Rural is $34.62. Meanwhile the average fare per driver for Urban cities is $16.57, for Suburban is $39.50 and for Rural is $55.49. Hence, it is more profitable to work in Rural cities than it is in Urban cities. However, is important to note that the Suburban range of average fare and per driver fare is very close, which can let us to believe that the drivers in those cities have a higher guarantee of making the highest profit available. This may mean that it may take them less ride to make the average fare, that it is for Rural drivers. Again, this is just an assumption. 

![Pyber Summary](https://github.com/cynmmarin/PyBer_Analysis/blob/e29f75e41b9206bf48d6a97fa916ba45b135bf84/Images/PyBer_Summary.png)

Next, we will create a pivot table with the "date" as the index, the columns "type", and values "fare". This calculation will help us determine the relationship that fare prices and dates have on the "Total Fare by City Type".  By using the ÒlocÓ function, we will focus on the time frame between '2019-01-01':'2019-04-29'. The results go has follows:

1. All cities see a spike on late February and a drop in March
2. The total for Rural cities fares do not surpass $500, meanwhile the Suburban stays below $1,500 and the Urban fare goes as high as almost touching the $2,500.
3. All city types have very distinct fluctuations between March and April and there seems to be no significant patterns.
4. In April, both Urban and Rural seem to decrease while the Suburban has a drop but picks up and has a higher slope than the other two. 

![Pyber_fare_summary](https://github.com/cynmmarin/PyBer_Analysis/blob/e29f75e41b9206bf48d6a97fa916ba45b135bf84/Analysis/PyBer_fare_summary.png)

We can conclude that Mid-February is a good month for all tree city types, but late February is a negative month for the drivers. Also, Urban cities are the city type with the highest revenue and therefore the most desirable place for drivers to work in. 

## Summary 








