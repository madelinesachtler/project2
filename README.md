# Project 2 


## EXTRACT 
Country data was extracted from Kaggle.com
- We decided that it was easiest to collect datasets with a common column name. 
- We found three datasets that all included information about food, happiness and GDP all connected by the Country name. 
- We downloaded the csv files and imported them into Pandas, and subsquently formatted them into separate dataframes. 


## Transform 
A substantial amount of data cleaning was requried in order to create a dataframe that was worth keeping with interesting information.
- Once imported, we selected the relevant data for each country from each of the three dataframes.
- Rows with NaN values were dropped and whitespace was stripped from the "Country" columns.
- After cleaning each of the three unique dataframes, we merged each dataframe on "Country".
- After dropping remaining NaN rows, the final dataframe contained complete data for 116 different countries.

## Load  
Once we had created our cleaned dataframe, we modified the columns to be lower case in order for the database to correctly recognize the columns. It was necessary for the columns to also be in the correct order in both the database and the dataframes for it to be properly imported. 
- Created a config.py document that held my username and password for postgres without pulically uploading personal information. 
- Made sure that the data had imported into SQL correctly by using the SELECT * from function. 
