# Project_1

# 1 Project Idea

Is Washington Ready for the EV Revolution?

# 2 Data Source

https://rapidapi.com/letscrape-6bRBa3QguO5/api/ev-charge-finder
- Charging Location 

https://fueleconomy.gov/feg/tax2023.shtml
- Tax Incentives 2023

https://catalog.data.gov/dataset/electric-vehicle-population-data
- Washington State Data


# Group Members 
Esha Patel, Jeff Morgan, Ipsita Pattanaik, Smita Shah, Neil Lawren

### PROJECT OUTINE

* Select the real-world data set from API/any other source.
* Download the dataset and convert it into a Pandas DataFrame.
* Perform data cleaning/deal with missing values using Pandas and NumPy.
* Plot interactive graphs to understand the data using visual libraries like matplotlib and hvplot.
* Ask and Answer questions from the dataset.


# 3 Questions to be answered
1. Which cities in Washington have the most electric and hybrid cars registered?
2. What is the ratio of cars to chargers in the selected cities? 
    - fast/slow charging ports
3. What are the most popular car models in the selected cities and do they have federal rebate?

# Analysis
### QUESTION 1 ANALYSIS: Which cities in Washington have the most electric and hybrid cars registered?
#### Data Overview:
-	Total Rows: 159,106
-	Analysis Focus: Electric and Plug-in Hybrid Vehicles in Washington State, Top 5 Cities 

#### Data Analysis Steps:
-	Grouped data by city and state.
-	Counted VIN (1-10) for each city.
-	Identified top 5 cities with the highest counts.
-	Filtered cities with more than 5000 registered cars.

#### Top 5 Cities with most Electric Vechicles:
-	Bothell, Vancouver, Redmond, Bellevue, and Seattle.

#### Visualizations:
##### Bar Chart 1: Top 5 Cities with Highest EV and Plug-in-hybrid Cars Registered
-	Represents the top 5 cities based on registered electric and plug-in hybrid vehicles.

##### Bar Chart 2: Total Chargers Available by Cities
-	Represents the total number of chargers available in the top 5 cities. The bar chart helps indicates the charging infrastructure in these cities.

#### Analysis: 
-	The analysis provides a view of the distribution of electric and hybrid vehicles in Washington State.
-	Bothell, Vancouver, Redmond, Bellevue, and Seattle emerge as key cities with significant car registrations.
-	The charging infrastructure is visualized through the total number of chargers in these cities.
-	This analysis provides insights into the distribution of electric and plug-in hybrid vehicles and the corresponding charging infrastructure in the specified top 5 cities in Washington State with highest number of registered All-Electric Cars and Plug-In-hybrid cars.

### QUESTION 2 ANALYSIS: What is the ratio of cars to chargers in the selected cities? What is the speed for all the chargers in top 5 cities?
#### Reading Data:
-	The data is read from a CSV file and stored in the chargers_df DataFrame.

#### Filtering Data:
-	We have executed filters on the data for charging stations located in Bellevue, Bothell, Seattle, Vancouver, and Redmond, WA and storeed it in the relevant variables. 

#### Pie Chart:
-A pie chart is created to visualize the distribution of charging speeds for the selected top 5 cities with the greatest population of electric vehicles. 
- A pie chart was also created to show charger distribution for the selected top 5 cities with the greatest population of electric vehicles. 
-	The charging_speed_counts variable stores the count of each charging speed category in the filtered data.
-	The pie chart is created using Matplotlib with labeled slices, colors, and other styling options.

#### Map Plot:
- A map plot using hvplot.points is created to display the availability of charging stations on a map for top selected cities. 

#### Analysis: 
- The analysis shows that overall the top 5 cities has slow chargers. ....

### QUESTION 3 ANALYSIS: Question 3: What are the most popular car models in the selected cities have federal rebate?
#### Reading Data:
-	The data is read from a CSV file and stored in the tax_rebate_per_model_compressed_df Dataframe.

#### Merging Data:
-	We have merged the tax rebate data with our top 5 cities dataframe to calculate total for all top car models for selected 5 cities.

#### Bar Chart: Most Popular Car Models in all 5 Cities and WordCloud:
-	Represents the top 6 car models for all selected cities.

#### Analysis: 
- Based on our analysis, the most popular car choosen by buyers in selected cities is the TESLA Model Y it also has a federal incentive of $7500. We found that not all electric cars are eligible for federal tax incentive. 

### MAIN ANALYSIS: OVERALL QUESTION!!!!


