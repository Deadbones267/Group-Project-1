# Analyzing Energy Consumption, Cost Efficiency, and Resource Utilization in U.S. States Based on Weather and Climate Impacts

## Project Statement
Understanding the effectiveness and efficiency of various energy sources across different U.S. regions is crucial for optimizing energy policies and consumption patterns. Weather, climate, and regional supply and demand dynamics significantly influence energy costs and availability. The Geographical Energy Consumption Analysis Tool created for this project was designed to help consumers analyze energy consumption patterns, costs, and resource utilization across U.S. states and regions, with a particular focus on how weather and climate affect energy consumption and efficiency.

## The Geographical Energy Consumption Analysis Tool
The Geographical Energy Consumption Analysis Tool is an application designed to evaluate how weather patterns in various locations impact energy consumption. The application relies on historical energy data from the [U.S. Energy Information Administration (EIA)](https://www.eia.gov/opendata/browser/) and historical weather data from [Open-Meteo](https://open-meteo.com/en/docs/historical-weather-api).

## Programming Language and Technology
The Geographical Energy Consumption Analysis Tool is written in [Python](https://www.python.org/) using [Visual Studio Code](https://code.visualstudio.com/) and the [JSON](https://www.json.org/json-en.html) data interchange format.


Visualizations are provided through the use of [Matplotlib](https://matplotlib.org/) and [Prophet](https://pypi.org/project/prophet/).


Energy statistics and analysis information were retrieved from [EIA](https://www.eia.gov/opendata/browser/) and weather information was retrieved from [Open-Meteo](https://open-meteo.com/en/docs/historical-weather-api).


The [Pandas](https://pandas.pydata.org/) and [Numpy](https://numpy.org/) libraries were used to work with the historical weather and energy data retrieved from the [U.S. Energy Information Administration (EIA)](https://www.eia.gov/opendata/browser/), [Open-Meteo](https://open-meteo.com/en/docs/historical-weather-api), and [Geoapify](https://www.geoapify.com/) APIs.

## Installation Guide

The contents of the repository should be placed into the desired folder on the user's computer, being sure to maintain the directory structure. 

The application was developed using Python version 3.12.4. Other versions of Python may work, but no guarantee is made. We suggest using a new virtual environment with the correct version of Python.

The following Python packages must be installed to run the application locally:

* matplotlib
* numpy
* pandas
* prophet
* jupyterlab (only if the .ipynb file is used. running the .py file does not require jupyterlab)

These packages may be individually installed into the environment of your choice. You will also need to obtain an API key for the EIA API and store it as eia in a file named local_keys.env. Alternatively, you may enter your EIA API key into the code manually, if desired. Additionally, you will need to obtain an API key from Geoapify and store it in your local_keys.env file as geo.

## Objectives
This project aims to identify the most and least cost-effective energy sources across U.S. regions by comparing costs based on supply, demand, and resource availability. It will analyze how weather patterns influence energy consumption, highlighting regions with higher energy use due to climate variability, and assess regional efficiency in using renewable versus non-renewable sources.

1. **Cost-Effectiveness Analysis of Energy Sources**:
   - Identify the most and least cost-effective energy sources (e.g., natural gas, solar, wind, coal, nuclear) in different U.S. states or regions.
   - Compare energy costs across regions, taking into account supply, demand, and resource availability.

2. **Impact of Weather and Climate on Energy Consumption**:
   - Analyze how weather patterns (e.g., temperature, seasonal changes, extreme weather events) affect energy consumption and efficiency.
   - Determine if certain regions experience higher energy costs or consumption due to weather variability (e.g., regions with colder winters or hotter summers).

3. **Resource Utilization and Energy Policy Implications**:
   - Evaluate which regions are using renewable vs. non-renewable energy sources more efficiently and at lower costs.
   - Provide insights into how weather/climate conditions should be factored into energy policies for each state or region.

## Initial Research Questions
  - How do weather and climate affect energy consumption in different U.S. states?
  - Which energy sources are the most cost-effective in regions with extreme weather (e.g., cold winters, hot summers)?
  - How does regional supply and demand influence the availability and price of different energy sources?
  - What role do renewable energy sources play in reducing energy costs and increasing efficiency, particularly in regions with favorable weather conditions (e.g., sunny, windy states)?
  - How do different energy policies across states impact energy costs and consumption patterns?

## Data Sources

For Energy:
  - EIA Open Data API: [U.S. Energy Information Administration (EIA)](https://www.eia.gov/opendata/browser/)

For Geolocation:
  - Geoapify API: [https://www.geoapify.com/]
    
For Weather:
  - Weather API: [Open-Meteo](https://open-meteo.com/en/docs/historical-weather-api)

## Initial Visualization Goals

**Electricity Consumption vs. Temperature by Region**

Graph Type: Line graph or scatter plot
X-Axis: Average monthly temperature (°F or °C)
Y-Axis: Monthly electricity consumption (KWh)
Data: Plot this for different U.S. states or regions over a year to show how temperature changes affect electricity usage.
Insights: This graph can reveal how temperature extremes (hot summers, cold winters) drive higher energy consumption, particularly for heating and cooling.

## Application Output Examples

The code is designed to plot the average monthly temperatures against energy consumption by geographic location. The sample output for this visualization will look like the following plot:
![image](https://github.com/user-attachments/assets/d0a5b8d2-b908-42bd-a05b-9a493cdf2327)

Additionally, the code is designed to run a Prophet model based on the 5-year historical trend to predict 24 months of energy utilization data. The sample Prophet model output looks like this:

![image](https://github.com/user-attachments/assets/c85c7a3f-3bfb-40ca-8c51-89a8acece257)


## Future Work and Visualizations

Future work and/or recommended enhancements to this project include:
* Implementing a regional model that allows users to view weather patterns and energy utilization trends by geographic region
* Evaluating how various types of energy impact energy costs
* Analyzing energy utilization by sector (commercial, residential, etc.)
* Evaluating the effect of climate change on energy consumption

**Renewable Energy Generation vs. Wind Speed/Solar Radiation**

Graph Type: Scatter plot or bubble chart
X-Axis: Wind speed (m/s) or solar radiation (W/m²)
Y-Axis: Renewable energy generation (MWh)
Bubble Size/Color: Energy type (e.g., wind, solar)
Data: Use hourly or daily data from regions with significant wind or solar generation.
Insights: This graph highlights the efficiency of renewable energy production as a function of local weather conditions, showing the correlation between natural resources and energy output.

**Energy Cost vs. Climate Events (Heatwaves, Cold Snaps, Hurricanes)**

Graph Type: Bar graph or time series plot
X-Axis: Timeline (years/months)
Y-Axis: Energy cost ($ per MWh)
Overlay: Mark specific extreme weather events (e.g., heatwaves, hurricanes) on the timeline
Data: Use cost data before, during, and after major climate events.
Insights: This graph helps show how extreme weather events can cause spikes in energy costs due to increased demand or infrastructure damage.

**Carbon Emissions from Energy Sources vs. Average Annual Temperature**

Graph Type: Line or stacked bar graph
X-Axis: Average annual temperature (°F or °C)
Y-Axis: Carbon emissions (metric tons CO₂)
Data: Break down emissions by energy source (coal, natural gas, renewables) for each state or region.
Insights: This can demonstrate how regions with higher temperatures or climate variability contribute to carbon emissions, and how the energy mix influences those emissions.

**Energy Production vs. Precipitation Levels**

Graph Type: Dual-axis line graph
X-Axis: Time (months or years)
Y-Axis (Left): Energy production from hydropower (MWh)
Y-Axis (Right): Monthly/annual precipitation levels (inches or mm)
Data: Plot energy production in regions with significant hydropower plants, like the Pacific Northwest, alongside precipitation data.
Insights: This graph could highlight how rainfall variability affects hydropower generation and how water resources impact energy availability.

**Energy Consumption Growth vs. Climate Change Indicators (Temperature Rise, CO₂ Levels)**

Graph Type: Line graph or area chart
X-Axis: Time (years or decades)
Y-Axis (Left): Total energy consumption (MWh)
Y-Axis (Right): Global CO₂ levels (ppm) or average global temperature anomaly (°C)
Data: Use long-term data for global CO₂ levels, temperature rise, and U.S. or regional energy consumption.
Insights: This graph visualizes the relationship between growing energy consumption and increasing climate change indicators, revealing how human energy use may be contributing to global warming.

## Link to Presentation
https://www.canva.com/design/DAGS7iinPiE/Ok38zvA45MSe5U-R4F1nHg/view?utm_content=DA[…]re_your_design&utm_medium=link&utm_source=shareyourdesignpanel

## Contributors
* [Keri Alexander](https://github.com/kerialexander)
* [JD](https://github.com/spidercousin)
* [Ian Hale](https://github.com/hollidaydds)
* [Reis Hymer](https://github.com/Doobles1989)
* [Carson Jones](https://github.com/Deadbones267)

