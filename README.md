# Weather & Vacation Analysis

Enable travellers to select their ideal vacation location based on various weather parameters by visually and statistically showing the relationship between latitude and certain weather conditions.

Specifically, provide real-time suggestions for clients' ideal hotels, where "ideal" is defined as hotels:

- Within a given range of latitude and longitude and
- That provide the right kind of weather for the client

## Project Plan

- **Task:** Collect and analyze weather data across cities worldwide.
- **Purpose:** Enable travel planning site to use data to recommend ideal hotels based on clients' weather preferences.
- **Method**: Create a Pandas DataFrame with 500 or more of the world's unique cities and their weather data in real time. This process will entail collecting, analyzing, and visualizing the data.

## Data Analysis

### Collect the Data

- Use the NumPy module to generate more than 1,500 random latitudes and longitudes.
- Use the citipy module to list the nearest city to the latitudes and longitudes.
- Use the OpenWeatherMap API to request the current weather data from each unique city in your list.
- Parse the JSON data from the API request.
- Collect the following data from the JSON file and add it to a DataFrame:
    - City, country, and date
    - Latitude and longitude
    - Maximum temperature
    - Humidity
    - Cloudiness
    - Wind speed

### Exploratory Analysis with Visualization

- Create scatterplots, determine correlations, and create a series of heatmaps using the Google Maps and Places API for the following comparisons:
    - Latitude vs. temperature
    - Latitude vs. humidity
    - Latitude vs. cloudiness
    - Latitude vs. wind speed

### Visualize Travel Data

Create a heatmap with pop-up markers that can display information on specific cities based on a customer's travel preferences. Complete these steps:

1. Filter the Pandas DataFrame based on user inputs for a minimum and maximum temperature.
2. Create a heatmap for the new DataFrame.
3. Find a hotel from the cities' coordinates using Google's Maps and Places API, and Search Nearby feature.
4. Store the name of the first hotel in the DataFrame.
5. Add pop-up markers to the heatmap that display information about the city, current maximum temperature, and a hotel in the city.