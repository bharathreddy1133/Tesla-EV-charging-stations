## Analysis of Tesla EV Charging Stations in New York State

---
## Task List

| ID | Task Description | Due Date | Status |
| --- | --- | --- | --- |
| 1 | Update this table with detailed list of tasks | 2023-05-08 | DONE |
| 2 | Extract API data in json format (importing data into pandas dataframe) | 2023-05-02 | DONE |
| 3 | Merging of two API with JSON format (Using 'usecols') | 2023-05-04 | DONE |
| 3 | Identifying outliers (Null values, data entry errors) | 2023-05-05 | DONE |
| 4 | Data Manipulation (Filtering, sorting, merging data, removing duplicates, reshaping data) | 2023-05-05 | DONE |
| 5 | Gain insights with descriptive statistics (summarising, aggregating data with respect to cities and counties) | 2023-05-05 | DONE |
| 6 | Data Visualization with matlplotlib and geopandas (Using folium library-heatmap, interactive maps) | 2023-05-07 | DONE |
| 7 | Determine the areas with highest demand for EV charging  | 2023-05-10 | DONE |
| 8 | Identifying opportunities for improvement | 2023-05-12 | DONE |
| 9 | Compile results from analysis | 2023-05-14 | DONE |
| 10 | Complete YouTube video and upload to YouTube | 2023-05-16 | DONE |
| 11 | Upload README.md document to Github | 2023-05-17 | DONE |

 
### Option 2 - Online Data Analysis
#### Data Sources
https://data.ny.gov/Energy-Environment/Electric-Vehicle-Charging-Stations-in-New-York/7rrd-248n/data

This dataset includes details such as the Distribution of charging stations across the New York state, Availability of charging stations by time of day, Type of charging stations, Status of charging stations, in detail name of the station, street address, city, state, ZIP code, phone number, latitude and longitude of the location, status code, access details, and the date when the information was last confirmed.

https://data.ny.gov/Economic-Development/Census-2010-and-2020-Population-Cities/dnpm-m8w3

The Census 2010 and 2020 Population dataset, provided by the State of New York, contains population data for cities and towns in the state of New York. The dataset includes population counts for the years 2010 and 2020, as well as the change in population between those years. From this dataset we have extracted 2020 population census data for the Exploratory data analysis.

#### Analysis Plan
**- Identifying outliers:**
To identify outliers, we will start by visualizing the data using scatter plots or box plots. Outliers will be data points that are significantly different from the rest of the data points. Once outliers are identified, we will investigate why they exist and if they are due to data entry errors or actual anomalous situations.

The analysis plan involves identifying interesting outliers in the data, to analyze the distribution and availability of EV charging stations in New York State.
Objective: Analyzing the Electric Vehicle (EV) charging station data for New York State to gain insights into the state of EV charging infrastructure and inform future development.
Points:
- Determine the total number of EV charging stations in New York State and track changes over time.
- Identify the most popular types of charging stations in New York State.
- Calculate the average distance between charging stations in different regions of New York State.
- Identify the counties with the most and least EV charging stations.
- Identify the cities with the highest demand for EV charging stations.


**- Exploratory Data Analysis (EDA):**
We will conduct exploratory data analysis, which involves using descriptive statistics, data visualization, and other techniques to identify patterns and trends in the data of EV charging stations in New York State. This can include examining the distribution and availability of charging stations by location, time, type, and status. We can also analyze the average distance between charging stations in different regions and identify outliers and potential reasons for their existence. EDA will help us gain insights into the state of EV charging infrastructure in New York State and inform future development to support the growth of the EV industry.

**- Determining the areas with highest demand for EV Charging:**
The data will be analysed to identify the areas with the highest demand for EV charging stations, the most popular types of charging stations, and any other trends that may emerge from the data. Using the dataset, we want to determine the optimal location of charging stations in New York State to minimize the cost of installing and operating them while ensuring that all areas are covered, considering the factors such as the number of EVs in each area, the distance between charging stations, and the types of charging stations needed (Level 2 or DC Fast).

Overall, the analysis of the EV charging station data for New York State is expected to contribute to the development of a more robust and efficient EV charging infrastructure in the state from our analysis.

**Note**- *Based on a preliminary analysis of the data and the modules learned in class, we have developed an initial set of outcomes from the data. As we conduct further analysis, we will incorporate additional points into our analysis plan, which will be detailed in the final project report.*

#### Motivation
The motivation of the project is to analyze the current state of EV charging infrastructure in New York State and identify areas for improvement. As more and more people are adopting electric vehicles, there is a growing need for an efficient and reliable charging network to support them. By analysing the data on EV charging stations in New York State, the project aims to provide insights into the distribution, availability, and demand for charging stations. The project also aims to inform future development of the charging infrastructure and contribute to the growth of electric mobility in the state.

YouTube Video:  [Link](https://youtu.be/0gXMewIA_XY)

## Introduction
Imagine you are driving your electric vehicle on a road trip through New York State, but you are running low on battery power, and you cannot find an EV charging station nearby. Frustrating, right? That is where our project comes in. By analysing the distribution and availability of EV charging stations in New York State, we aim to identify areas with the highest demand for charging stations and inform the development of a more efficient and accessible EV charging infrastructure. Our project can ultimately contribute to a more sustainable and eco-friendly future for all.

With the data on Electric Vehicle Charging Stations and Census 2020 Population, we are conducting several types of analysis to gain insights into the distribution, availability, and demand for EV charging stations in New York State.

Firstly, we are identifying outliers in the data to investigate why they exist and if they are due to data entry errors or actual anomalous situations.
Next, we are conducting exploratory data analysis (EDA) using descriptive statistics, data visualization, and other techniques to identify patterns and trends in the data of EV charging stations in New York State. This can include examining the distribution and availability of charging stations by location, time, type, and status. EDA will help us gain insights into the state of EV charging infrastructure in New York State and inform future development to support the growth of the EV industry.

We are also determining the areas with the highest demand for EV Charging and identifying the most popular types of charging stations in New York State. By analyzing the data, we aim to determine the optimal location of charging stations in New York State to minimize the cost of installing and operating them while ensuring that all areas are covered, considering factors such as the number of EVs in each area, the distance between charging stations, and the types of charging stations needed (Level 2 or DC Fast). Overall, we aim to provide insights into the state of the EV charging infrastructure in New York State and identify areas for improvement. This project also aims to inform future development of the charging infrastructure and contribute to the growth of electric mobility in the state.

---

## References
The code retrieves data the following sources
- Electric Vehicle Charging Stations in New York: https://data.ny.gov/Energy-Environment/Electric-Vehicle-Charging-Stations-in-New-York/7rrd-248n/data
- Census 2010 and 2020 Population: https://data.ny.gov/Economic-Development/Census-2010-and-2020-Population-Cities/dnpm-m8w3
The data was retrieved from these sources using the data APIs provided by the State of New York.

---

## Requirements
To run the code in this project, these prerequisite Python packages/libraries should be installed:
- Pandas: This library is used for data manipulation and analysis. This can be installed by running the command ‘pip install pandas’.
- Requests: The Requests library is a popular Python library for making HTTP requests to web servers. It simplifies the process of sending HTTP/1.1 requests and handling the responses by abstracting away much of the low-level details of the protocol. This can be installed by running the command ‘pip install requests’.
- Numpy: This library is used for scientific computing and working with arrays. This can be installed by running the command ‘pip install numpy’.
- Matplotlib: This library is used for data visualization and plotting. This can be installed by running the command ‘pip install matplotlib’.
- Folium: This library is used for creating interactive maps. This can be installed by running the command ‘pip install folium’.
- Geopy: This library is used for calculating distances between two points using their latitude and longitude coordinates. This can be installed by running the command ‘pip install geopy’.
- Seaborn: Seaborn is a Python data visualization library based on Matplotlib. It provides a high-level interface for creating informative and attractive statistical graphics. Seaborn can be used for exploring data, understanding relationships between variables, and creating complex visualizations. This can be installed by running the command ‘pip install seaborn’.

We did not use any API keys in the code snippets provided in this session. However, we used publicly available datasets from the New York State Open Data portal, which provides access to a variety of datasets including EV charging station locations, population data, and more.
To use the data from these datasets, we simply loaded them into pandas DataFrames using their URLs, cleaned them up as necessary, and then used them for analysis and visualization.


---

## Explanation of the Code

The code, `needs_a_good_name.py`, begins by importing necessary Python packages:

Fetching and Displaying Data from a JSON API using Pandas in Python
- First, we import the Pandas library and the requests library. Pandas is a library used for data manipulation and analysis, while requests are used for making HTTP requests.
- Next, we specify the URL of the website from which we want to extract data. In this case, we're using a New York State dataset from the data.ny.gov website.
- We then use the requests library to make an HTTP GET request to the specified URL and store the response in a variable called 'response'.
- After that, we extract the data from the response object in JSON format and store it in a variable called 'data'.
- We also extract the headers from the response object and store them in a variable called 'headers'.
- We then extract the column names from the headers object and store them in a list called 'column names'.
- Finally, we create a Pandas DataFrame using the data and column_names variables and store it in a variable called 'df'.
- We then print the DataFrame to the console using the 'print' function.
- And that's it! Running this code will extract data from the specified website and store it in a Pandas DataFrame for further analysis.

```
#Fetching and Displaying Data from a JSON API using Pandas in Python
# Import the necessary libraries
import pandas as pd  # Library for data manipulation and analysis
import requests  # Library for making HTTP requests
# Specify the URL of the website from which we want to extract data
url = 'https://data.ny.gov/api/views/7rrd-248n/rows.json'
# Use the requests library to make an HTTP GET request to the specified URL and store the response in a variable called 'response'
response = requests.get(url)
# Extract the data from the response object in JSON format and store it in a variable called 'data'
data = response.json()['data']
# Extract the headers from the response object and store them in a variable called 'headers'
headers = response.json()['meta']['view']['columns']
# Extract the column names from the headers object and store them in a list called 'column_names'
column_names = [header['name'] for header in headers]
# Create a Pandas DataFrame using the data and column_names variables and store it in a variable called 'df'
df = pd.DataFrame(data, columns=column_names)
# Print the DataFrame to the console using the 'print' function
print(df)
```
We get the output for the raw data as below
<img width="784" alt="#Fetching and Displaying Data from a JSON API using Pandas in Python" src="https://github.com/IE-555/final-project-PFA_Final/assets/124125241/bc299e40-4536-41f8-8a61-d55c48f50e7b">



Extracting and Displaying Electric Vehicle Charging Station Data from a CSV file Using Pandas (Filtering)

- The script starts by importing the pandas and requests libraries. Then, it sets the URL of the dataset we want to use to a variable called url.
- Instead of reading a CSV file like in the original code, we'll use the requests.get function to retrieve the data from the URL as a JSON object. We'll then extract the data and columns elements from the JSON object, and use them to create a pandas DataFrame called df. This allows us to work with the data more easily, and use functions like dropna to filter out missing values.
- Once we have the DataFrame, we can extract each column of data by assigning them to their own variables. For example, we can assign the "Station Name" column to a variable called station_name, and so on.
- Next, we can use the dropna function to display only the non-NaN values for each column. We do this for each column, printing the column name and the non-NaN values below it.
-	Now, let's take a closer look at how we can group and analyze the data. First, we'll group the data by city using the groupby function, and then count the number of unique stations in each city using the nunique function. We'll assign the results to a variable called station_counts.
-	Finally, we can print the station_counts variable to display the results
-	And that's it! With just a few lines of code, we've downloaded and analyzed data on electric vehicle charging stations in New York State using pandas and requests.

```
#Extracting and filtering New York State Ev Stations Dataset (filtering)
# import required libraries
import pandas as pd
import requests
# specify the URL of the data source
url = 'https://data.ny.gov/api/views/7rrd-248n/rows.json'
# make a GET request to the API endpoint and store the response
response = requests.get(url)
# parse the response as JSON and extract the data and column headers
data = response.json()['data']
headers = response.json()['meta']['view']['columns']
# extract the column names from the headers
column_names = [header['name'] for header in headers]
# create a pandas DataFrame from the data and column names
df = pd.DataFrame(data, columns=column_names)
# print the station name column with NaN values dropped
print("Station Name:")
print(df["Station Name"].dropna())
print()

```
<img width="797" alt="#Extracting and filtering New York State Ev Stations Dataset" src="https://github.com/IE-555/final-project-PFA_Final/assets/124125241/cf46f203-879a-4821-b108-5854a533a321">


Loading Census Population Data from a URL using Pandas in Python

-	Let's start by importing the Pandas library using the import statement.
-	Then, we create a variable url to store the URL where the Census population data is located.
-	We use the pd.read_csv function to read the CSV data from the URL and store it in a Pandas dataframe called data.
-	Finally, we use the print function to print the data to the console.
-	That's it! With just a few lines of code, we've loaded Census population data from a URL using Pandas in Python.

```
# import the pandas library
import pandas as pd

# specify the URL of the CSV file to read
url = "https://data.ny.gov/api/views/dnpm-m8w3/rows.csv?accessType=DOWNLOAD"

# use the read_csv() function from pandas to read the CSV file from the URL
data = pd.read_csv(url)

# print the contents of the CSV file to the console
print(data)
```
<img width="782" alt="#Loading Census Population Data from a URL using Pandas in Python" src="https://github.com/IE-555/final-project-PFA_Final/assets/124125241/50d62c19-82bb-4d7e-a7ad-3bd60b38916b">

Extracting and filtering New York State 2020 Census population data using pandas

-	The first step is to import the Pandas library using the "import pandas as pd" command. This will allow us to use Pandas to read and manipulate the dataset.
-	Next, we'll load the dataset from the CSV file using the "pd.read_csv()" method. We'll pass the URL of the dataset as the argument to the method.
-	Once the dataset is loaded, we'll filter it to include only the "2020 Census Population" and "Area Name" columns using the "df[["2020 Census Population", "Area Name"]]" command. We'll store the filtered dataset in a new variable called "df_filtered".
-	Finally, we'll print the filtered dataset using the "print()" command. This will display only the "2020 Census Population" and "Area Name" columns.
```
import pandas as pd
# Load the dataset from the CSV file
df = pd.read_csv("https://data.ny.gov/api/views/dnpm-m8w3/rows.csv?accessType=DOWNLOAD")
# Filter the dataset to include only the "2020 Census Population" and "Area Name" columns
df_filtered = df[["2020 Census Population", "Area Name"]]
# Print the filtered dataset
print(df_filtered.to_string(index=False))
```
<img width="530" alt="image" src="https://github.com/IE-555/final-project-PFA_Final/assets/124185765/ffe7bc8f-7c48-4136-a18b-41b1cf91cf07">

Grouping and Counting Unique Values in a Pandas DataFrame using Python

- We begin by importing the necessary libraries for this project. pandas is a powerful data analysis library that provides data structures and tools for working with tabular data, and requests is a library for making HTTP requests in Python.
- Next, we define the URL of the JSON API endpoint that contains the data we want to analyze. In this case, we are using a dataset provided by the New York State Department of Environmental Conservation that contains air quality monitoring station data.
- We then use the requests library to send a GET request to the API URL and get the response as JSON data. The json() method is called on the response object to convert the JSON data into a Python dictionary.
- We extract the data and headers from the JSON response by accessing the "data" and "meta.view.columns" keys of the dictionary, respectively. We use a list comprehension to extract the names of the columns from the headers.
- We then create a Pandas DataFrame from the data and column names using the pd.DataFrame() constructor.
- We group the data by city using the groupby() method of the DataFrame, and count the number of unique stations in each city using the nunique() method.
- Finally, we loop over the resulting station_counts object, which is a Pandas Series with the cities as the index and the counts as the values. For each city and count pair, we print a formatted string that displays the city and count.
```
import pandas as pd
import requests
# Define the URL for the JSON API endpoint
url = 'https://data.ny.gov/api/views/7rrd-248n/rows.json'
# Send a GET request to the URL and get the response as JSON data
response = requests.get(url).json()
# Extract the data and headers from the response
data = response['data']
headers = response['meta']['view']['columns']
column_names = [header['name'] for header in headers]
# Create a DataFrame from the data and headers
df = pd.DataFrame(data, columns=column_names)
# Group the data by city and count the number of unique stations
station_counts = df.groupby("City")["Station Name"].nunique()
# Display the count of unique stations for all cities
for city, count in station_counts.items():
    print(f"{city}: {count}")
```
<img width="818" alt="#Grouping and Counting number of EV stations by city in a Pandas DataFrame using Python" src="https://github.com/IE-555/final-project-PFA_Final/assets/124125241/72a327d1-d6c5-4022-afe3-5531e5b1aab3">

Filtering Data and Creating a Map of EV Stations in New York State using Pandas and Folium in Python.

- We'll be using the New York State Open Data API, which provides access to a wide variety of data sets in JSON format. Specifically, we'll be using the API endpoint for the dataset of EV charging stations, which provides information on the location, type, and availability of charging stations in the state."
- First, we define the API endpoint URL and make a GET request to the API to get the JSON data. Then, we parse the JSON data into a DataFrame using the pd.DataFrame constructor from the pandas library. Finally, we create a map object centered on New York and add markers to the map for each EV charging station in the DataFrame."
- To create the map, we'll be using the Folium library, which provides an easy way to create interactive maps in Python. Here's the code that creates the map and adds markers to it. First, we create a map object centered on New York using the folium.Map constructor. Then, we iterate over each row in the DataFrame and add a marker to the map for each EV charging station using the folium.Marker constructor."
```
import folium
import pandas as pd
import requests
# Define the API endpoint URL
url = 'https://data.ny.gov/api/views/7rrd-248n/rows.json'
# Make a GET request to the API endpoint and get the JSON data
response = requests.get(url)
data = response.json()['data']
headers = response.json()['meta']['view']['columns']
column_names = [header['name'] for header in headers]
# Create a Pandas DataFrame from the JSON data
df = pd.DataFrame(data, columns=column_names)
# Filter out data points that are outside of New York State
df = df[df['State'] == 'NY']
# Create a map object centered on New York
ny_map = folium.Map(location=[40.7128, -74.0060], zoom_start=7)
# Iterate over each row in the DataFrame and add a marker for the EV station
for index, row in df.iterrows():
    # Get the latitude and longitude of the station
    lat, lon = float(row["Latitude"]), float(row["Longitude"])
    # Add a marker to the map at the location of the station
    folium.Marker(location=[lat, lon]).add_to(ny_map)
# Display the map
ny_map
```
<img width="745" alt="#Filtering Data and Creating a Map of EV Stations in New York State using Pandas and Folium in Python" src="https://github.com/IE-555/final-project-PFA_Final/assets/124125241/2129f3aa-0fcb-4ef4-8cc8-ccb08f255cb2">

Fetching and Displaying Filtered Data from a JSON API Using Pandas and Folium HeatMap in Python.

- We will begin by importing the Pandas and Folium libraries, as well as the HeatMap module from Folium. We will also import the requests library to fetch data from the JSON API.
- Next, we'll use the requests library to fetch data from the JSON API. We'll specify the URL of the API and use the response.json() method to convert the response to a JSON object. We'll then extract the data and header information from the JSON object and create a Pandas DataFrame from the data.
- We'll define a rectangular area that covers the boundaries of New York State and use it to filter out data points that fall outside of this area. We'll convert the Longitude and Latitude columns to float using the astype() method and then apply the filtering conditions using boolean indexing.
- We'll extract the Longitude and Latitude columns from the filtered DataFrame and create a Folium Map centered at New York City. We'll then create a HeatMap layer using the HeatMap() method and add it to the map using the add_to() method.
- Finally, we'll display the map using the map variable.
```
import pandas as pd
import folium
from folium.plugins import HeatMap
import requests
# Fetch data from the JSON API URL
url = 'https://data.ny.gov/api/views/7rrd-248n/rows.json'
response = requests.get(url)
data = response.json()['data']
headers = response.json()['meta']['view']['columns']
column_names = [header['name'] for header in headers]
df = pd.DataFrame(data, columns=column_names)
# Filter out data points outside of New York state
ny_coords = [-79.875366, 40.477399, -71.851682, 45.01585]
df = df[(df['Longitude'].astype(float) >= ny_coords[0]) &
        (df['Latitude'].astype(float) >= ny_coords[1]) &
        (df['Longitude'].astype(float) <= ny_coords[2]) &
        (df['Latitude'].astype(float) <= ny_coords[3])]
# Extract latitude and longitude columns
locations = df[["Latitude", "Longitude"]]
# Create a map centered at New York City
nyc_coords = (40.7128, -74.0060)
map = folium.Map(location=nyc_coords, zoom_start=10)
# Add a heatmap layer to the map
heatmap = HeatMap(data=locations, radius=10)
heatmap.add_to(map)
# Display the map
map
```
<img width="733" alt="#Fetching and Displaying Filtered Data from a JSON API Using Pandas and Folium HeatMap in Python" src="https://github.com/IE-555/final-project-PFA_Final/assets/124125241/098938fb-1fd7-40f3-a4c7-fcb6595d4c94">

Locating cities with most EV stations

- First, we import the Pandas and Folium libraries. Pandas is a popular library for working with data in Python, and Folium is a library for creating interactive maps.
- We then load the dataset from a CSV file using Pandas' read_csv() function. The CSV file contains information about electric vehicle charging stations in New York State, including the location, city, and station name.
- Next, we group the data by city and count the number of unique charging stations in each city using Pandas' groupby() and nunique() functions.
- Host: We then find the city with the maximum number of charging stations using the idxmax() function.
- Now that we have the city with the most charging stations, we can visualize the data on a map. We create a Folium map object centered on New York City.
- We then add a marker for each charging station in New York City using a for loop to iterate over each row in the dataset.
- Finally, we display the map on our screen using Folium's Map function.
```
import pandas as pd
import folium
# Load the dataset from the CSV file
df = pd.read_csv("https://data.ny.gov/api/views/7rrd-248n/rows.csv?accessType=DOWNLOAD")
# Group the data by city and count the number of unique stations
station_counts = df.groupby("City")["Station Name"].nunique()
# Find the city with the maximum number of charging stations
max_city = station_counts.idxmax()
# Create a map object centered on the maximum city
location = df.loc[df["City"] == max_city, ["Latitude", "Longitude"]].iloc[0]
map = folium.Map(location=[location[0], location[1]], zoom_start=11)
# Add a marker for each charging station
for index, row in df.iterrows():
    if row["City"] == max_city:
        lat, lon = row["Latitude"], row["Longitude"]
        folium.Marker(location=[lat, lon]).add_to(map)
# Display the map
map
```
<img width="737" alt="#Locating cities with most EV stations" src="https://github.com/IE-555/final-project-PFA_Final/assets/124125241/99cf789a-163c-4de5-a164-f8d928bce4b2">

Visualization of 2020 Census Population by New York City Area Name. (Bar Graph):

- First, we need to import the necessary libraries. We will be using Pandas to load and filter the data, and Matplotlib to create the bar chart.
- Next, we will load the data from the CSV file using the Pandas read_csv() function and store it in a DataFrame called df.
- Now, we will filter the data to only include the columns for the 2020 Census population and area name.
- We will sort the data by the 2020 Census population in descending order.
- Next, we will create the bar chart using Matplotlib. We will set the size of the figure to 50x50 inches using plt.figure(figsize=(50,50)).
- We will create the bars using plt.bar() and pass in the sorted area names and population values.
- We will rotate the x-axis labels by 90 degrees and set the font size to 6 using plt.xticks(rotation=90, fontsize=6.
- We will set the font size of the y-axis labels to 10 using plt.yticks(fontsize=10).
- We will add an x-axis label using plt.xlabel() and set the font size to 12.
- We will add a y-axis label using plt.ylabel() and set the font size to 12.
- Finally, we will add population numbers as text labels on the bars using plt.text(). We will iterate over the bars using a for loop and use the get_x(), get_width(), and get_height() methods to determine the coordinates of the labels. We will set the horizontal alignment to 'center', the vertical alignment to 'bottom', and the font size to 3.
- Finally, we will display the bar chart using plt.show().
```
import pandas as pd
import matplotlib.pyplot as plt
# Load the dataset from the CSV file
df = pd.read_csv("https://data.ny.gov/api/views/dnpm-m8w3/rows.csv?accessType=DOWNLOAD")
# Filter the dataset to only include 2020 Census Population and Area Name
df_filtered = df[["2020 Census Population", "Area Name"]]
# Sort the dataset by 2020 Census Population in descending order
df_sorted = df_filtered.sort_values(by=["2020 Census Population"], ascending=False)
# Create a bar chart to visualize the 2020 Census Population for each city
plt.figure(figsize=(50,50))
bars = plt.bar(df_sorted["Area Name"], df_sorted["2020 Census Population"], width=0.8)
plt.xticks(rotation=90, fontsize=6)
plt.yticks(fontsize=10)
plt.xlabel("Area Name", fontsize=12)
plt.ylabel("2020 Census Population", fontsize=12)
plt.title("2020 Census Population by Area Name", fontsize=14)
# Add population numbers as text labels on the bars
for i, bar in enumerate(bars):
    plt.text(bar.get_x() + bar.get_width() / 2, bar.get_height() + 1000, str(df_sorted.iloc[i]["2020 Census Population"]), ha='center', va='bottom', fontsize=3)
plt.show()
```
<img width="755" alt="#Visualization of 2020 Census Population by New York City Area Name  (Bar Graph)" src="https://github.com/IE-555/final-project-PFA_Final/assets/124125241/07b0930c-7365-44ef-967e-086ff211b4d9">

Pie Chart of 2020 Census Population by Area Name in New York State:

-	First, we need to import the Pandas and Matplotlib libraries.
-	Next, we load the dataset from the CSV file using Pandas
-	We then filter the dataset to only include the 2020 Census Population and Area Name columns.
-	To get a better view of the data, we sort the dataset by the 2020 Census Population in descending order.
-	"Finally, we create a pie chart to visualize the 2020 Census Population for each city."
```
import pandas as pd
import matplotlib.pyplot as plt
# Load the dataset from the CSV file
df = pd.read_csv("https://data.ny.gov/api/views/dnpm-m8w3/rows.csv?accessType=DOWNLOAD")
# Filter the dataset to only include 2020 Census Population and Area Name
df_filtered = df[["2020 Census Population", "Area Name"]]
# Sort the dataset by 2020 Census Population in descending order
df_sorted = df_filtered.sort_values(by=["2020 Census Population"], ascending=False)
# Create a pie chart to visualize the 2020 Census Population for each city
plt.figure(figsize=(50,50))
plt.pie(df_sorted["2020 Census Population"], labels=df_sorted["Area Name"], autopct='%1.1f%%', textprops={'fontsize':6})
plt.title("2020 Census Population by Area Name")
plt.show()
```
<img width="824" alt="#Pie Chart of 2020 Census Population by Area Name in New York State" src="https://github.com/IE-555/final-project-PFA_Final/assets/124125241/3b40ba68-2715-44fe-989a-4224ee3b3780">

Estimated Number of EV Stations Needed in Each City:

-	First, we need to import the panda’s library for data manipulation and analysis, python.
-	we will load the dataset from a CSV file and filter it to include only the columns we need - the 2020 Census population and the name of each city.
-	We also need to define the target number of EV stations per capita. In this example, we will use one station per 15,000 people.
-	Using this target ratio, we can calculate the estimated number of EV stations needed for each city by multiplying the population by the target ratio and rounding to the nearest whole number.
-	Finally, we can display the result in a table format by simply printing the data frame.
```
import pandas as pd
from IPython.display import display
# Load the dataset from the CSV file and filter it to include only the desired columns
df = pd.read_csv("https://data.ny.gov/api/views/dnpm-m8w3/rows.csv?accessType=DOWNLOAD", 
                 usecols=["2020 Census Population", "Area Name"])
pd.set_option("display.max_rows", None)
# Define the target number of EV stations per capita
target_stations_per_capita = 0.0015  # 1 station per 15,000 people
# Calculate the estimated number of EV stations needed for each city
df["Estimated EV Stations"] = (df["2020 Census Population"] * target_stations_per_capita).round()
# Display the result in a table
display(df)
```
<img width="416" alt="#Estimated Number of EV Stations Needed in Each City" src="https://github.com/IE-555/final-project-PFA_Final/assets/124125241/cb28e469-1e04-49f8-b51e-2d1c2c849605">

Combined analysis of current EV stations and estimated EV stations per capita in NY cities

-	we need to import the pandas and requests libraries to work with the datasets and make API calls to the New York State Open Data portal. We also import the numpy library to work with numerical data.
-	Next, we define the URL for the JSON API endpoint of the "Electric Vehicle Supply Equipment Locations in New York State" dataset, and we send a GET request to the URL to get the data as JSON. We then extract the data and headers from the response and create a pandas DataFrame from them. We group the data by city and count the number of unique stations for each city, and we save the result in a pandas Series called station_counts.
-	We now load the "Census 2010 and 2020 Population (Cities and Towns)" dataset from the New York State Open Data portal, using the read_csv function from pandas. We filter the dataset to include only the columns for the 2020 census population and the city/town name, and we calculate the estimated number of EV stations needed per capita using a target ratio of 1 station per 15,000 people.
-	We merge the two datasets on the city/town name column, and we drop any rows with missing values (NaNs). We also combine the names of cities/towns with multiple words into a single string. Finally, we display the result as a panda DataFrame with the estimated number of EV stations and the current number of unique stations for each city/town
```
import pandas as pd
import requests
# Define the URL for the JSON API endpoint
url = 'https://data.ny.gov/api/views/7rrd-248n/rows.json'
# Send a GET request to the URL and get the response as JSON data
response = requests.get(url).json()
# Extract the data and headers from the response
data = response['data']
headers = response['meta']['view']['columns']
column_names = [header['name'] for header in headers]
# Create a DataFrame from the data and headers
df = pd.DataFrame(data, columns=column_names)
# Group the data by city and count the number of unique stations
station_counts = df.groupby("City")["Station Name"].nunique().reset_index(name='EV Stations')
# Remove NaN values
station_counts.dropna(inplace=True)
# Load the dataset from the CSV file and filter it to include only the desired columns
census_df = pd.read_csv("https://data.ny.gov/api/views/dnpm-m8w3/rows.csv?accessType=DOWNLOAD", 
                        usecols=["2020 Census Population", "Area Name"])
# Combine city names
census_df["Area Name"] = census_df["Area Name"].str.replace(" city", "").str.replace(" town", "")
station_counts["City"] = station_counts["City"].str.replace(" city", "").str.replace(" town", "")
# Merge the station counts and census data on city names
merged_df = pd.merge(station_counts, census_df, left_on="City", right_on="Area Name", how="inner")
# Define the target number of EV stations per capita
target_stations_per_capita = 0.0015  # 1 station per 10,000 people
# Calculate the estimated number of EV stations needed for each city
merged_df["Estimated EV Stations"] = (merged_df["2020 Census Population"] * target_stations_per_capita).round()
# Display the result
print(merged_df[["City", "EV Stations", "Estimated EV Stations"]])
```
<img width="598" alt="image" src="https://github.com/IE-555/final-project-PFA_Final/assets/124125241/086e41cc-171d-43d8-b6b4-16eef2dd3b22">

Analyzing Electric Vehicle Charging Station Data in New York State Max & Min Station

- The first step is to import the Pandas library using the "import pandas as pd" command. This will allow us to use Pandas to read and manipulate the dataset.
- Next, we'll load the dataset from the CSV file using the "pd.read_csv()" method. We'll pass the URL of the dataset as the argument to the method.
-	Once the dataset is loaded, we'll filter it to include only the "2020 Census Population" and "Area Name" columns using the "df[["2020 Census Population", "Area Name"]]" command. We'll store the filtered dataset in a new variable called "df_filtered".
- Finally, we'll print the filtered dataset using the "print()" command. This will display only the "2020 Census Population" and "Area Name" columns.
```
import pandas as pd
# Load the dataset from the CSV file
df = pd.read_csv("https://data.ny.gov/api/views/dnpm-m8w3/rows.csv?accessType=DOWNLOAD")
# Filter the dataset to include only the "2020 Census Population" and "Area Name" columns
df_filtered = df[["2020 Census Population", "Area Name"]]
# Print the filtered dataset
print(df_filtered.to_string(index=False))
```
<img width="511" alt="#Extracting and filtering New York State 2020 Census population data using pandas" src="https://github.com/IE-555/final-project-PFA_Final/assets/124125241/89aade11-ea6f-4189-9533-9d5ca492f9af">

Analyzing Electric Vehicle Charging Station Data in New York State Max & Min Station

-	Now that we have our data loaded into a DataFrame, we can start exploring it. Let's begin by taking a look First, we'll load the EV station data into a pandas DataFrame using the URL provided by the data source. Then, we'll group the data by city and count the number of unique stations in each city.
-	Next, we'll use the idxmax() and idxmin() methods to find the city with the most and least charging stations, respectively. We'll also store the corresponding counts for each city.
-	Finally, we'll print out the results to the console, including the names of the cities and their respective station counts.
```
#Analyzing Electric Vehicle Charging Station Data in New York State Max & Min Station
import pandas as pd
# Load the EV station dataset into a pandas DataFrame
ev_url = "https://data.ny.gov/api/views/7rrd-248n/rows.csv?accessType=DOWNLOAD"
ev_df = pd.read_csv(ev_url)
# Group the EV station data by city and count the number of unique stations
station_counts = ev_df.groupby("City")["Station Name"].nunique()
# Get the city with the most charging stations
max_station_city = station_counts.idxmax()
max_station_count = station_counts[max_station_city]
# Get the city with the least charging stations
min_station_city = station_counts.idxmin()
min_station_count = station_counts[min_station_city]
# Print the results
print(f"The city with the most EV charging stations is {max_station_city} with {max_station_count} stations.")
print(f"The city with the least EV charging stations is {min_station_city} with {min_station_count} stations.")
```
<img width="575" alt="image" src="https://github.com/IE-555/final-project-PFA_Final/assets/124125241/4d3b1a83-3b8f-48da-9026-90ba8bf5cc94">

Calculating Total Number of Electric Vehicle Charging Stations in New York State

- Import the necessary library: The code begins by importing the pandas library using the import pandas as pd statement. This library provides data manipulation and analysis tools in Python.
- Define the URL for the EV station dataset: The variable ev_url stores the URL pointing to the CSV file containing the EV station data. In this example, it uses the New York State EV station dataset from the specified URL.
- Load the EV station dataset into a pandas DataFrame: The pd.read_csv() function is used to read the CSV file from the specified URL and create a pandas DataFrame named ev_df. The DataFrame is a tabular data structure that allows for easy manipulation and analysis of the data.
- Calculate the total number of EV stations: The code then calculates the total number of EV stations by summing the values in three columns of the DataFrame: "EV Level1 EVSE Num", "EV Level2 EVSE Num", and "EV DC Fast Count". The .sum() method is used to sum the values in each column, and the results are added together.
- Print the total number of EV stations: Finally, the code uses the print() function to display the total number of EV stations calculated in the previous step. It uses an f-string (f"Total number of EV stations: {total_ev_stations}") to format the output and include the value of total_ev_stations in the printed message.
```
import pandas as pd
# Load the EV station dataset into a pandas DataFrame
ev_url = "https://data.ny.gov/api/views/7rrd-248n/rows.csv?accessType=DOWNLOAD"
ev_df = pd.read_csv(ev_url)
# Sum the values in the "EV Level1 EVSE Num", "EV Level2 EVSE Num", and "EV DC Fast Count" columns
# to get the total number of EV stations
total_ev_stations = ev_df["EV Level1 EVSE Num"].sum() + ev_df["EV Level2 EVSE Num"].sum() + ev_df["EV DC Fast Count"].sum()
# Print the total number of EV stations
print(f"Total number of EV stations: {total_ev_stations}")
```
<img width="236" alt="image" src="https://github.com/IE-555/final-project-PFA_Final/assets/124125241/d2af736d-b903-4986-a933-62e7052aba57">

Calculating Total Number of Electric Vehicle Charging Stations by Type in New York State

- Loading the EV station dataset To start, we will load the EV station dataset into a pandas DataFrame using the API endpoint.
- Analyzing the number of Level 1 charging stations We will filter the data to include only Level 1 EVSE stations and sum the values in the "EV Level1 EVSE Num" column to get the total number of Level 1 EVSE stations.
- Analyzing the number of Level 2 charging stations Next, we will filter the data to include only Level 2 EVSE stations and sum the values in the "EV Level2 EVSE Num" column to get the total number of Level 2 EVSE stations.
- Analyzing the number of DC Fast Charge stations Lastly, we will filter the data to include only DC Fast Charge stations and sum the values in the "EV DC Fast Count" column to get the total number of DC Fast Charge stations.
- And there you have it, we have analyzed the number of EV charging stations in New York and categorized them by level. As the popularity of electric vehicles continues to grow, it is crucial to have sufficient charging stations to support them
```
import pandas as pd
# Load the EV station dataset into a pandas DataFrame
ev_url = "https://data.ny.gov/api/views/7rrd-248n/rows.csv?accessType=DOWNLOAD"
ev_df = pd.read_csv(ev_url)
# Filter the data to include only Level 1 EVSE stations
level1_df = ev_df[ev_df["EV Level1 EVSE Num"] > 0]
# Sum the values in the "EV Level1 EVSE Num" column to get the total number of Level 1 EVSE stations
total_level1_stations = level1_df["EV Level1 EVSE Num"].sum()
# Filter the data to include only Level 2 EVSE stations
level2_df = ev_df[ev_df["EV Level2 EVSE Num"] > 0]
# Sum the values in the "EV Level2 EVSE Num" column to get the total number of Level 2 EVSE stations
total_level2_stations = level2_df["EV Level2 EVSE Num"].sum()
# Filter the data to include only DC Fast Charge stations
dc_fast_df = ev_df[ev_df["EV DC Fast Count"] > 0]
# Sum the values in the "EV DC Fast Count" column to get the total number of DC Fast Charge stations
total_dc_fast_stations = dc_fast_df["EV DC Fast Count"].sum()
# Print the total number of Level 1, Level 2, and DC Fast Charge stations
print(f"Total number of Level 1 EVSE stations: {total_level1_stations}")
print(f"Total number of Level 2 EVSE stations: {total_level2_stations}")
print(f"Total number of DC Fast Charge stations: {total_dc_fast_stations}")
```
<img width="329" alt="image" src="https://github.com/IE-555/final-project-PFA_Final/assets/124125241/15772230-c941-4a22-a9c0-780b72393775">

Visualizing the Total Number of EV Stations by Level

- import pandas as pd: This imports the pandas library and assigns it the alias 'pd' for easier reference.
- import matplotlib.pyplot as plt: This imports the pyplot module from the matplotlib library and assigns it the alias 'plt' for easier reference.
- ev_url = "https://data.ny.gov/api/views/7rrd-248n/rows.csv?accessType=DOWNLOAD": This assigns the URL of the EV station dataset to the variable ev_url.
- ev_df = pd.read_csv(ev_url): This uses pandas' read_csv() function to read the CSV data from the URL and create a DataFrame called ev_df to store the data.
- level1_df = ev_df[ev_df["EV Level1 EVSE Num"] > 0]: This creates a new DataFrame called level1_df by filtering ev_df to include only rows where the "EV Level1 EVSE Num" column is greater than 0.
- level2_df = ev_df[ev_df["EV Level2 EVSE Num"] > 0]: This creates a new DataFrame called level2_df by filtering ev_df to include only rows where the "EV Level2 EVSE Num" column is greater than 0.
- dc_fast_df = ev_df[ev_df["EV DC Fast Count"] > 0]: This creates a new DataFrame called dc_fast_df by filtering ev_df to include only rows where the "EV DC Fast Count" column is greater than 0.
- total_level1_stations = level1_df["EV Level1 EVSE Num"].sum(): This calculates the total number of Level 1 stations by summing the values in the "EV Level1 EVSE Num" column of level1_df.
- total_level2_stations = level2_df["EV Level2 EVSE Num"].sum(): This calculates the total number of Level 2 stations by summing the values in the "EV Level2 EVSE Num" column of level2_df.
- total_dc_fast_stations = dc_fast_df["EV DC Fast Count"].sum(): This calculates the total number of DC Fast Charge stations by summing the values in the "EV DC Fast Count" column of dc_fast_df.
- labels = ["Level 1", "Level 2", "DC Fast Charge"]: This creates a list called labels containing the labels for the different station levels.
- values = [total_level1_stations, total_level2_stations, total_dc_fast_stations]: This creates a list called values containing the total number of stations for each level.
- plt.bar(labels, values): This creates a bar graph using matplotlib's bar() function, using the labels and values lists as the x-axis and y-axis data, respectively.
- plt.title("Total Number of EV Stations by Level"): This sets the title of the graph to "Total Number of EV Stations by Level".
- plt.xlabel("EV Station Level"): This sets the label for the x-axis of the graph to "EV Station Level".
- plt.ylabel("Number of Stations"): This sets the label for the y-axis of the graph to "Number of Stations".
- plt.show(): This displays the graph on the screen.
```
import pandas as pd
import matplotlib.pyplot as plt
# Load the EV station dataset into a pandas DataFrame
ev_url = "https://data.ny.gov/api/views/7rrd-248n/rows.csv?accessType=DOWNLOAD"
ev_df = pd.read_csv(ev_url)
# Filter the data to include only Level 1, Level 2, and DC Fast Charge stations
level1_df = ev_df[ev_df["EV Level1 EVSE Num"] > 0]
level2_df = ev_df[ev_df["EV Level2 EVSE Num"] > 0]
dc_fast_df = ev_df[ev_df["EV DC Fast Count"] > 0]
# Sum the values in each column to get the total number of stations
total_level1_stations = level1_df["EV Level1 EVSE Num"].sum()
total_level2_stations = level2_df["EV Level2 EVSE Num"].sum()
total_dc_fast_stations = dc_fast_df["EV DC Fast Count"].sum()
# Create a list of labels and a list of values for the bar graph
labels = ["Level 1", "Level 2", "DC Fast Charge"]
values = [total_level1_stations, total_level2_stations, total_dc_fast_stations]
# Create a bar graph using matplotlib
plt.bar(labels, values)
# Set the title and axis labels
plt.title("Total Number of EV Stations by Level")
plt.xlabel("EV Station Level")
plt.ylabel("Number of Stations")
# Show the graph
plt.show()
```
<img width="548" alt="image" src="https://github.com/IE-555/final-project-PFA_Final/assets/124125241/3b9f7952-d1ce-4a7e-9c1b-20b13d6ddaa4">

Creating a Heatmap to Visualize EV Station Shortage by City

- we'll be analyzing electric vehicle (EV) station data for cities in New York State. Specifically, we'll be looking at the difference between the actual and estimated number of EV stations per capita for each city.
- To begin, we'll import the necessary libraries and modules. We'll use pandas for data manipulation, requests for making API requests, seaborn for visualizations, and matplotlib for creating plots. [Code for library imports]
- Next, we'll calculate the difference between the actual and estimated number of EV stations per capita for each city. This will give us an idea of the EV station shortage for each city. [Code for calculating station shortage]
- Now, we'll create a pivot table with city names as the index and the station shortage as the values. We'll use this pivot table to create a heatmap that visualizes the station shortage for each city. [Code for creating pivot table and heatmap]
- We'll customize the heatmap by setting the theme to "coolwarm", adding annotations to the heatmap cells, and setting the figure size to 10x10. We'll also add a title, x-axis label, and y-axis label. [Code for customizing heatmap]
- Finally, we'll show the heatmap. 
```
import pandas as pd
import requests
import seaborn as sns
import matplotlib.pyplot as plt
# Calculate the difference between actual and estimated number of EV stations per capita
merged_df["Station Shortage"] = merged_df["Estimated EV Stations"] - merged_df["EV Stations"]
# Create a pivot table with city names as index and station shortage as values
heatmap_df = pd.pivot_table(merged_df, values="Station Shortage", index="City")
# Plot the heat map
sns.set_theme()
plt.figure(figsize=(10, 10))
sns.heatmap(heatmap_df, cmap="coolwarm", annot=True, fmt=".0f", linewidths=.5)
plt.title("EV Station Shortage by City")
plt.xlabel("Estimated EV Stations - Actual EV Stations")
plt.ylabel("City")
plt.show()
```
<img width="711" alt="image" src="https://github.com/IE-555/final-project-PFA_Final/assets/124125241/63628d0a-86ee-41b7-8c85-07226aa8ae2d">

Determine the total number of EV charging stations in New York State and track changes over time

-	we'll load the data from the CSV file that contains information about EV charging stations in New York State. We'll also set the 'Date Last Confirmed' column as the index.
-	Now that we have the data, we can group it by year and count the number of stations in each year.
-	We can now create a line plot of the yearly counts using Matplotlib.
-	Total Number of EV Charging Stations in New York State" is displayed as the title of the graph. The horizontal axis displays the year, and the vertical axis displays the number of stations. The plot shows the trend of the total number of EV charging stations over time.
```
import pandas as pd
import matplotlib.pyplot as plt
# Load the data from the CSV file
url = 'https://data.ny.gov/api/views/7rrd-248n/rows.csv?accessType=DOWNLOAD'
df = pd.read_csv(url, parse_dates=['Date Last Confirmed'])
# Set the 'Date Last Confirmed' column as the index
df.set_index('Date Last Confirmed', inplace=True)
# Group the data by year and count the number of stations
yearly_counts = df.groupby(pd.Grouper(freq='Y'))['Station Name'].count()
# Create a line plot of the yearly counts
yearly_counts.plot(kind='line', figsize=(20, 10))
# Set the title and axis labels
plt.title('Total Number of EV Charging Stations in New York State')
plt.xlabel('Year')
plt.ylabel('Number of Stations')
# Show the plot
plt.show()
```
<img width="814" alt="image" src="https://github.com/IE-555/final-project-PFA_Final/assets/124125241/648f2354-b881-4b94-af3d-090adf51c704">

Average distance between charging stations for each city

- First, we import the necessary libraries - pandas and geopy.
-	We then load the dataset of EV charging stations in New York State from a CSV file hosted on the web using the read_csv() function from pandas.
-	Next, we group the charging stations by city using the groupby() method from pandas.
-	We then iterate over each city group to calculate the average distance between charging stations using the geopy.distance library.
-	We print out the average distance between charging stations for each city using a formatted string.
-	By calculating the average distance between charging stations for each city, we can get an idea of how accessible charging stations are for EV drivers in different parts of the state
```
import pandas as pd
from geopy.distance import distance
# Load the EV station dataset into a pandas DataFrame
ev_url = "https://data.ny.gov/api/views/7rrd-248n/rows.csv?accessType=DOWNLOAD"
ev_df = pd.read_csv(ev_url)
# Group the EV station data by city
grouped = ev_df.groupby("City")
# Calculate the average distance between stations for each city
for city, group in grouped:
    # Calculate the distance between each station in the city
    distances = []
    for i in range(len(group)):
        for j in range(i+1, len(group)):
            # Extract the latitude and longitude of each station
            lat1 = group.iloc[i]["Latitude"]
            lon1 = group.iloc[i]["Longitude"]
            lat2 = group.iloc[j]["Latitude"]
            lon2 = group.iloc[j]["Longitude"]
            # Calculate the distance between the two stations using the geopy package
            dist = distance((lat1, lon1), (lat2, lon2)).miles
            distances.append(dist)
    # Calculate the average distance between stations for the city
    if len(distances) > 0:
        avg_distance = sum(distances) / len(distances)
        print(f"Average distance between stations in {city}: {round(avg_distance, 2)} miles")
```
<img width="611" alt="image" src="https://github.com/IE-555/final-project-PFA_Final/assets/124125241/13928075-a85c-47ec-a818-3dd6ff637aa4">

Identify the cities with the highest demand for EV charging stations.

Line 1: import pandas as pd
- This line imports the pandas library and assigns it the shorthand name "pd" for convenience. Pandas is a popular Python library for data manipulation and analysis.
- ev_url = "https://data.ny.gov/api/views/7rrd-248n/rows.csv?accessType=DOWNLOAD"
- This line defines a variable ev_url that stores a URL string pointing to a CSV file that contains data on electric vehicle charging stations in New York State.
ev_df = pd.read_csv(ev_url)
This line reads the CSV file at the URL specified by ev_url and stores the resulting data in a pandas DataFrame called ev_df.
- pop_url = "https://data.ny.gov/api/views/dnpm-m8w3/rows.csv?accessType=DOWNLOAD"
This line defines a variable pop_url that stores a URL string pointing to a CSV file that contains population data for New York State.
- pop_df = pd.read_csv(pop_url, usecols=["2020 Census Population", "Area Name"])
This line reads the CSV file at the URL specified by pop_url and stores the resulting data in a pandas DataFrame called pop_df. The usecols argument specifies that only the "2020 Census Population" and "Area Name" columns should be read.
- ev_df["City"] = ev_df["City"].str.replace(" city", "").str.replace(" town", "") and pop_df["Area Name"] = pop_df["Area Name"].str.replace(" city", "").str.replace(" town", "")
- These lines clean up the city names in the ev_df and pop_df DataFrames by removing the "city" and "town" suffixes.
- station_counts = ev_df.groupby("City").size().reset_index(name="EV Stations")
This line groups the ev_df DataFrame by city name and counts the number of rows (which corresponds to the number of EV charging stations) in each group. The resulting counts are stored in a new DataFrame called station_counts, which has two columns: "City" and "EV Stations".
- merged_df = pd.merge(station_counts, pop_df, left_on="City", right_on="Area Name")
This line merges the station_counts and pop_df DataFrames on the "City" and "Area Name" columns, respectively. The result is a new DataFrame called merged_df that contains the number of EV charging stations and population data for each city.
- merged_df["Stations per Capita"] = merged_df["EV Stations"] / merged_df["2020 Census Population"]
This line calculates the ratio of EV charging stations per capita for each city by dividing the number of charging stations in each city by the corresponding population size. The resulting ratios are added as a new column called "Stations per Capita" in the merged_df DataFrame.
- sorted_df = merged_df.sort_values("Stations per Capita", ascending=False)
This line sorts the merged_df DataFrame in descending order based on the "Stations per Capita" column, which gives the cities with the highest demand for EV charging stations.
- threshold = sorted_df["Stations per Capita"].quantile(0.90)
```
import pandas as pd
# Load the EV station and population datasets into pandas DataFrames
ev_url = "https://data.ny.gov/api/views/7rrd-248n/rows.csv?accessType=DOWNLOAD"
ev_df = pd.read_csv(ev_url)
pop_url = "https://data.ny.gov/api/views/dnpm-m8w3/rows.csv?accessType=DOWNLOAD"
pop_df = pd.read_csv(pop_url, usecols=["2020 Census Population", "Area Name"])
# Clean up the city names
ev_df["City"] = ev_df["City"].str.replace(" city", "").str.replace(" town", "")
pop_df["Area Name"] = pop_df["Area Name"].str.replace(" city", "").str.replace(" town", "")
# Group the EV station data by city and count the number of stations in each city
station_counts = ev_df.groupby("City").size().reset_index(name="EV Stations")
# Merge the station counts and population data on city names
merged_df = pd.merge(station_counts, pop_df, left_on="City", right_on="Area Name")
# Calculate the ratio of EV stations per capita for each city
merged_df["Stations per Capita"] = merged_df["EV Stations"] / merged_df["2020 Census Population"]
# Sort the cities in descending order based on the ratio of EV stations per capita
sorted_df = merged_df.sort_values("Stations per Capita", ascending=False)
# Display only the cities with the highest ratio of EV stations per capita
threshold = sorted_df["Stations per Capita"].quantile(0.90)
high_demand_cities = sorted_df[sorted_df["Stations per Capita"] > threshold]["City"]
print("Cities with the highest demand for EV charging stations:")
print(high_demand_cities.to_string(index=False))
```
<img width="386" alt="image" src="https://github.com/IE-555/final-project-PFA_Final/assets/124125241/1a4b59d8-730f-4a9d-80dd-b8c5d068e446">

Displaying the cities which are in high demand of EV

-	we will import the necessary libraries, including Folium and Pandas, and load the EV station and population datasets into Pandas data frames.
-	will then clean up the city names in both data frames to make them consistent.
-	we will group the EV station data by city and count the number of stations in each city.
-	We will merge the station counts and population data on city names to calculate the ratio of EV stations per capita for each city.
-	Then we will sort the cities in descending order based on the ratio of EV stations per capita and select the top 10 cities with the highest ratio of EV stations per capita.
-	Now we can create a map centered on New York State using Folium
- 	We will add a circle marker for each city with the size and color based on the number of EV stations. The tooltip will display the name of the city and the number of EV stations.
```
import folium
import pandas as pd
# Load the EV station and population datasets into pandas DataFrames
ev_url = "https://data.ny.gov/api/views/7rrd-248n/rows.csv?accessType=DOWNLOAD"
ev_df = pd.read_csv(ev_url)
pop_url = "https://data.ny.gov/api/views/dnpm-m8w3/rows.csv?accessType=DOWNLOAD"
pop_df = pd.read_csv(pop_url, usecols=["2020 Census Population", "Area Name"])
# Clean up the city names
ev_df["City"] = ev_df["City"].str.replace(" city", "").str.replace(" town", "")
pop_df["Area Name"] = pop_df["Area Name"].str.replace(" city", "").str.replace(" town", "")
# Group the EV station data by city and count the number of stations in each city
station_counts = ev_df.groupby("City").size().reset_index(name="EV Stations")
# Merge the station counts and population data on city names
merged_df = pd.merge(station_counts, pop_df, left_on="City", right_on="Area Name")
# Calculate the ratio of EV stations per capita for each city
merged_df["Stations per Capita"] = merged_df["EV Stations"] / merged_df["2020 Census Population"]
# Sort the cities in descending order based on the ratio of EV stations per capita
sorted_df = merged_df.sort_values("Stations per Capita", ascending=False)
# Select the top 10 cities with the highest ratio of EV stations per capita
top_cities = sorted_df.head(10)
# Create a map centered on New York State
ny_coords = (42.99, -75.44)
ev_map = folium.Map(location=ny_coords, zoom_start=7)
# Add a circle marker for each city with the size and color based on the number of EV stations
for i, row in top_cities.iterrows():
    city = row["City"]
    stations = row["EV Stations"]
    lat = ev_df.loc[ev_df["City"] == city, "Latitude"].mean()
    lon = ev_df.loc[ev_df["City"] == city, "Longitude"].mean()
    folium.CircleMarker(location=(lat, lon), radius=stations/2, color="blue", fill=True, fill_opacity=0.5, tooltip=f"{city}: {stations} EV Stations").add_to(ev_map)
# Display the map
ev_map
```
<img width="735" alt="image" src="https://github.com/IE-555/final-project-PFA_Final/assets/124125241/8a6cc5c7-7497-4a1a-886f-f807a39272c5">


## How to Run the Code

1. Download the required Python files: Download the Python files (.py) that contain the code for your analysis. Make sure to save them in a directory accessible from Jupyter Notebook.

2. Launch Jupyter Notebook: Open your command prompt or terminal and navigate to the directory where you saved the Python files. Then run the command jupyter notebook. This will launch Jupyter Notebook in your web browser.

3. Create a new Jupyter Notebook: Click on the "New" button in the top right corner of the Jupyter Notebook interface and select "Python 3" to create a new notebook.

4. Import the necessary files: In the first cell of your notebook, import the Python files containing the code. You can use the import statement to import the required files.This project file name is  NY_EV_CS_ANALYSIS.py (For Example import NY_EV_CS_ANALYSIS.py)

5. Run the code cells: Write or copy the code for your analysis into subsequent cells and run them by pressing Shift + Enter. Make sure to run the cells in the correct order if there are dependencies between them.

6. Review the results: The output of the code will be displayed below each code cell. You can review the results, including data visualizations and any insights or findings generated by the analysis.

---

## Results from the Analysis
- With the preliminary analysis, we have found these fields (Columns) in the EV station dataset with the size 3378 rows x 39 columns.
Station Name, Street address, city, latitude, longitude, zip code, Type of stations- EV level1 EVSE Num, EV level2 EVSE Num, EV DC Fast Count, Updated At (updated date of the station), Open date(start date of the station), EV Network (EV station provider), EV Network Web (Website link for the EV station), EV connector types.
- The dataset of 2020 population of New York has the size 61 rows x 6 columns. 
- We have found out the number of EV stations in each city of New York State.
  Currently, New York city has the most number of EV stations with 371 and Amagansett has the least number and least usage with only 1 EV station.
- Based on the census data, it has been determined that New York City comprises 75% of the population of New York state.
- With leaflet maps using folium library we have found out that there are three outliers in the EV station dataset. These are outliers in the latitude and longitude which are marked out of NY state.
- We have also plotted the cities with the most number of EV stations with leaflet maps.

**From the heatmap, we have interpreted the following**

- Density of EV Charging Stations: The heat map visually represents the density of EV charging stations in New York State. Areas with a higher concentration of charging stations will appear as hotter spots on the map, indicating higher demand or availability of charging infrastructure.
New York City, Albany City, Buffalo have the highest density of EV stations.

- Charging Station Deserts: Areas with fewer or no charging stations will appear as cooler spots on the map. This can help identify regions or communities that may have limited access to charging infrastructure and may require further development to support electric vehicle adoption. The heat map can assist in strategic planning for the expansion of charging infrastructure.

**From the Actual vs Estimated Analysis, we have interpreted the following**

- Discrepancy between Estimated and Actual EV Stations: We can observe that for some cities, the estimated number of EV stations differs significantly from the actual number. For example, cities like Albany, Amsterdam, Auburn, Batavia, and Beacon have a relatively lower number of actual EV stations compared to the estimated demand. This suggests that there might be a need for further investment and expansion of charging infrastructure in these cities to meet the growing demand.

- Higher Actual EV Stations: On the other hand, cities like Buffalo, Ithaca, Rochester, Saratoga Springs, Schenectady, Syracuse, and Yonkers have a higher number of actual EV stations compared to the estimated demand. This indicates that these cities have made significant efforts to develop their EV charging infrastructure and are better equipped to cater to the needs of EV owners.

- Population and EV Stations: While population size is not directly correlated with the number of EV stations, we can observe that cities with larger populations tend to have more EV stations. However, it is important to consider the estimated demand per capita to ensure sufficient charging infrastructure availability.

- Potential Opportunities: The analysis highlights potential opportunities for expanding EV charging infrastructure in cities where the estimated demand exceeds the actual number of EV stations. These cities may benefit from increased investment, partnerships with charging network providers, and government support to encourage EV adoption and improve charging accessibility.

**From the type of EV charging stations analysis**

- Total number of Level 1 EVSE (Electric Vehicle Supply Equipment) stations: 7.0
- Total number of Level 2 EVSE stations: 8182.0
- Total number of DC (Direct Current) Fast Charge stations: 1235.0
- These numbers represent the count of each type of charging station available in the given dataset. Level 1 EVSE stations provide the slowest charging speed, Level 2 EVSE stations offer a faster charging rate, and DC Fast Charge stations provide the fastest charging option for electric vehicles. These figures give an overview of the distribution of charging infrastructure types, indicating the availability and accessibility of different charging options for electric vehicle owners. It highlights the prominence of Level 2 EVSE stations, which are widely deployed and provide a reasonable charging speed for many EVs. Additionally, the presence of DC Fast Charge stations indicates the availability of high-speed charging options for EVs that support fast-charging capabilities.
- The average distance between stations in different locations varies significantly, ranging from very short distances to several miles. Some locations have very short average distances between stations, such as Arlington, Athens, Bolton Landing, Borough Park, and Frankfort, indicating that the stations are likely to be close to each other or even overlapping. On the other hand, some locations have relatively long average distances between stations, such as Cortland, Croton-on-Hudson, East Syracuse, Jamesville, and Jamestown. These locations may have stations spread out over a larger area.
- There are several locations where the average distance between stations is minimal or zero, suggesting that the stations may be located very close together or even at the same location. Examples include Altamont, Bolton, Castleton-on-Hudson, Dobbs Ferry, Greenport, Kinderhook, Long Island City, and North Tonawanda. Albany, Buffalo, Manhattan, and New York City have relatively larger average distances between stations, which is expected given the larger size and population density of these areas.
There are a few locations where the average distance between stations is quite large compared to others, such as Cortland, Jamestown, and Jamesville. These locations may have fewer stations or cover larger rural areas.
- The average distance between stations can provide insights into the accessibility and coverage of the transportation system in each location. Smaller average distances between stations may indicate a more dense and accessible network, while larger distances may suggest more limited coverage.

By selecting cities with a ratio higher than the 90th percentile threshold, the code identifies the cities that are in the top 10% in terms of the ratio of EV stations per capita. These cities are considered to have a higher demand for EV charging stations compared to the majority of cities in the dataset.
The output will consist of the following cities:
Hudson
Watervliet
Saratoga Springs
Kingston
Albany
Cohoes
These cities are identified as having the highest demand for EV charging stations based on the provided data. It's important to note that the analysis is specific to the dataset used and may not reflect the overall demand for EV charging stations globally or in other regions.

**What worked well**

**Data sources:** The selection of the Electric Vehicle Charging Stations dataset and the Census 2020 Population dataset provides a comprehensive foundation for analyzing the EV charging infrastructure in New York State. These datasets contain relevant information that allows for meaningful insights and analysis.

**Analysis objectives:** The project's objectives, such as determining the total number of EV charging stations, identifying popular types of charging stations, and analyzing demand in different areas, are well-defined and aligned with the goal of understanding the state of EV charging infrastructure.

**Analysis plan:** The analysis plan is well-structured, outlining steps for identifying outliers, conducting exploratory data analysis, and determining areas with high demand for EV charging. The plan covers various aspects of the data and analysis, which will likely provide comprehensive insights.

**What could be improved**

**Data cleaning:** The code performs basic data cleaning by removing certain substrings from the city names. However, there might be additional cleaning steps required, such as handling uppercase/lowercase inconsistencies, removing leading/trailing whitespaces, or handling special characters.

**Efficiency:** Depending on the size of the datasets, the code's efficiency could be improved. For example, it might be more efficient to filter and clean the data earlier in the process to reduce unnecessary computations. Additionally, optimizing operations like merging, grouping, and sorting could improve overall performance.

**Statistical Analysis:** The current analysis calculates the ratio of EV stations per capita to determine the cities with the highest demand. Consider incorporating additional statistical analysis techniques to validate the findings and explore potential correlations with other variables such as demographics or electric vehicle adoption rates.

