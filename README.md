# county-recommendation-engine

## Description of Data Used in Project
The detailed county-level housing data has been collected from Zillow. This includes information about property values, rental values, changes in home prices, etc...
This data can be downloaded individually from this page:<br>
https://www.zillow.com/research/data/

There is a very useful lookup table between zip codes, county names, state names, and FIPS codes on Kaggle. This was posted by Dan Ofer and can be found on this page:<br>
https://www.kaggle.com/danofer/zipcodes-county-fips-crosswalk

There is a very useful dataset which has been compiled by Mike Johnson Jr on Kaggle. This contains information for counties about the number, and type, of crimes committed in each county across years. This can be found on this page:<br>
https://www.kaggle.com/mikejohnsonjr/united-states-crime-rates-by-county

The US Department of Agriculture has compiled a code for each US county as to its rural to urban characteristics. This ranges from 1 to 9, where 1 is a major metropolitan city and 9 is completely rural. This can be found on this page:<br>
https://www.ers.usda.gov/data-products/rural-urban-continuum-codes//

From the US Department of Agriculture there is a very good dataset containing the unemployment rate and mean household income for each county. This can be found on this page:<br>
https://www.ers.usda.gov/data-products/county-level-data-sets/download-data/

Uber has released information on the average ride lengths for 7 cities in the United States. While my project does not specifically focus on ride-sharing or public transport, there is something very important which can be gleaned from this. Here I use this data with the assumption that the average length of time in takes to get from somewhere inside a county to somewhere inside a county you want to go is similar whether you are taking Uber or driving your own car. I know this is not entirely correct, and carries significant bias, but we can still glean very important information for this. I hope that eventually, through partnerships with other companies, I can expand this information to cover the entire country. I grabbed information for hours of the day mean travel times on weekdays and weekends. These datasets can be navigated to from this page:<br>
https://movement.uber.com/cities?lang=en-US

# Order to Run Notebooks
Eventually these will be combined into a streamlined app, but for now (to understand how they build on each other) please follow these in the following order.
1. Run 'Munging at County Level.ipyng'
2. Run 'Pre-Processing County DF.ipynb'
3. Run 'Pre_Process_Traffic_Data.ipynb'
4. Run 'Incorporate Traffic Information.ipynb'
5. Run 'county-recommendation-engine.ipynb'
6. Run 'Time_Series_Prediction.ipynb'
