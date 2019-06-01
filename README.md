# Housing-prices
## Does good weather increase apartment prices?
In numerous conversations about buying an apartment in Sweden have I heard comments like “I bet people are willing to give more for the apartment on a sunny day” or “The bidding has driven up price so much today, must be the good weather”. Pondering to eventually buy an apartment in Stockholm one day, I became curious about the link between the final price of the apartment and the weather. To find out whether this link exists, I’ve scraped the listings of apartments sold in Stockholm between March and October 2018 and added data on cloudiness at the day of sale and took a closer look at prices and weather using Python. 

In short, _**I do not find evidence**_ that cloudiness is an important determinant of the final price. At least one less thing to be less strategic about when apartment hunting. 

## Data
To obtain data on prices and characteristics of apartments sold in Stockholm, I scraped listings of apartments sold from Sweden’s largest real estate portal https://www.hemnet.se/. 
My data span from March to October 2018. The available variables include final price for the apartment, area in square meters, monthly fee, amount of rooms, date of sale, and city area. 

Data on weather was downloaded from Swedish Meteorological and Hydrological Institute https://www.smhi.se/klimatdata. I choose daily cloudiness as the measure of weather. The cloudier, the worse is the weather. I’ve also replicated the analysis making use of precipitation data, but arrived to the same conclusion, i.e. rain is not a determinant of final price. 

## Overview of the results
Find full code for the analysis in Housing_prices_weather.ipynb.

Visual analysis of the normalized data makes it evident that **weather is not correlated** with the final price... 
![Image of H](/Heatmap.png)

... **nor is it a significant determinant** of final price.
![Image of O](/OLS_results_main.png)
