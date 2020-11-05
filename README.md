# Top_Cities_To_Own_Electric_Car

## Census

Our program starts by executing the Census_Population.ipynb file in the Census folder. This notebook performs the following operations:

1. Makes a call to the Census API for city and city population. The data that is retunred is stored in a dataframe called census_df.
2. Prints the total number of cities in the census_df dataset.
3. Creates a df called big_city_df which only includes cities where the population is over 250k.
4. Prints the number of big cities to the screen.
5. Creates a data frame names City_State which holds the values of the split city name so that city and state are in one columns.
6. Merges the big_city_df dataframe with the City_State dataframe in city_merge_df.
7. Renames the newly merged columns from City_State as Clean_City and Clean_State
8. Creates a new column in city_merge_df called City_State which is the concatenation of the column Clean_City and a comma and Clean_State. 
9. Creates blank columns for Lat and Lng in the city_merge_df
9. Loops trough city_merge_df and retrieves Lat and Lng by passing City_State to the api request.
10. Prints a log of what was loaded and what was not loaded to the screen.
11. Creates a df called final_city_df which holds columns for City_State, Clean_City, Population, Lat, and Lng.
12. Generates a csv file of the final_city_df to the Resources folder.
13. Generates a bar chart of the top 10 cities by largest population
14. Creates a heat map of the cities weighted by population.
15. Generates a boxplot of population.

## Weather



## OpenCharge
