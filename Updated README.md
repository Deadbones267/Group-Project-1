# Analyzing Energy Consumption, Cost Efficiency, and Resource Utilization in U.S. States Based on Weather and Climate Impacts

## PROJECT STATEMENT:
Understanding the effectiveness and efficiency of various energy sources across different U.S. regions is crucial for optimizing energy policies and consumption patterns. Weather, climate, and regional supply and demand dynamics significantly influence energy costs and availability. The Energy Consumption Analysis Tool created for this project was designed to help consumers analyze energy consumption patterns, costs, and resource utilization across U.S. states and regions, with a particular focus on how weather and climate affect energy consumption and efficiency.

The Energy Consumption Analysis Tool is an application designed to evaluate how weather patterns in various locations impact energy consumption. The application relies on historical energy data from [the U.S. Energy Information Administration (EIA)](https://www.eia.gov/opendata/browser/) and historical weather data from [Open-Meteo] (https://open-meteo.com/en/docs/historical-weather-api).

## Programming Language and Technology
The Energy Consumption Analysis Tool is written in [Python](https://www.python.org/) using [Visual Studio Code](https://code.visualstudio.com/).

Visualizations are provided through [Bokeh](https://bokeh.org/), [hvPlot](https://hvplot.holoviz.org/index.html), and Matplotlib

Energy statistics and analysis information was retrieved from [EIA API]()

The [Pandas](https://pandas.pydata.org/) and [Numpy] (https://numpy.org/) libraries were used to work with the historical weather and energy data retrieved from the EIA and Open-Meteo APIs.

## OBJECTIVES:
1. **Cost-Effectiveness Analysis of Energy Sources**:
   - Identify the most and least cost-effective energy sources (e.g., natural gas, solar, wind, coal, nuclear) in different U.S. states or regions.
   - Compare energy costs across regions, taking into account supply, demand, and resource availability.

2. **Impact of Weather and Climate on Energy Consumption**:
   - Analyze how weather patterns (e.g., temperature, seasonal changes, extreme weather events) affect energy consumption and efficiency.
   - Determine if certain regions experience higher energy costs or consumption due to weather variability (e.g., regions with colder winters or hotter summers).

3. **Resource Utilization and Energy Policy Implications**:
   - Evaluate which regions are using renewable vs. non-renewable energy sources more efficiently and at lower costs.
   - Provide insights into how weather/climate conditions should be factored into energy policies for each state or region.

## RESEARCH QUESTIONS:
  - How do weather and climate affect energy consumption in different U.S. states?
  - Which energy sources are the most cost-effective in regions with extreme weather (e.g., cold winters, hot summers)?
  - How does regional supply and demand influence the availability and price of different energy sources?
  - What role do renewable energy sources play in reducing energy costs and increasing efficiency, particularly in regions with favorable weather conditions (e.g., sunny, windy states)?
  - How do different energy policies across states impact energy costs and consumption patterns?

## POSSIBLE DATA SOURCES:

For Weather:
  - Weather API: https://open-meteo.com/en/docs/historical-weather-api#start_date=2000-01-01&end_date=2009-12-31&hourly=temperature_2m,relative_humidity_2m,precipitation&location_mode=csv_coordinates&temperature_unit=fahrenheit&wind_speed_unit=mph&precipitation_unit=inch


For Electricity:
  - EIA Open Data API: https://www.eia.gov/opendata/browser/
  - Electricity Maps API: https://static.electricitymaps.com/api/docs/index.html


## Visualization goals:

**_1. Electricity Consumption vs. Temperature by Region_**

Graph Type: Line graph or scatter plot
X-Axis: Average monthly temperature (°F or °C)
Y-Axis: Monthly electricity consumption (MWh)
Data: Plot this for different U.S. states or regions over a year to show how temperature changes affect electricity usage.
Insights: This graph can reveal how temperature extremes (hot summers, cold winters) drive higher energy consumption, particularly for heating and cooling.


**_2. Renewable Energy Generation vs. Wind Speed/Solar Radiation_**

Graph Type: Scatter plot or bubble chart
X-Axis: Wind speed (m/s) or solar radiation (W/m²)
Y-Axis: Renewable energy generation (MWh)
Bubble Size/Color: Energy type (e.g., wind, solar)
Data: Use hourly or daily data from regions with significant wind or solar generation.
Insights: This graph highlights the efficiency of renewable energy production as a function of local weather conditions, showing the correlation between natural resources and energy output.


**_3. Energy Cost vs. Climate Events (Heatwaves, Cold Snaps, Hurricanes)_**

Graph Type: Bar graph or time series plot
X-Axis: Timeline (years/months)
Y-Axis: Energy cost ($ per MWh)
Overlay: Mark specific extreme weather events (e.g., heatwaves, hurricanes) on the timeline
Data: Use cost data before, during, and after major climate events.
Insights: This graph helps show how extreme weather events can cause spikes in energy costs due to increased demand or infrastructure damage.


**_4. Carbon Emissions from Energy Sources vs. Average Annual Temperature_**

Graph Type: Line or stacked bar graph
X-Axis: Average annual temperature (°F or °C)
Y-Axis: Carbon emissions (metric tons CO₂)
Data: Break down emissions by energy source (coal, natural gas, renewables) for each state or region.
Insights: This can demonstrate how regions with higher temperatures or climate variability contribute to carbon emissions, and how the energy mix influences those emissions.


**_5. Energy Production vs. Precipitation Levels_**

Graph Type: Dual-axis line graph
X-Axis: Time (months or years)
Y-Axis (Left): Energy production from hydropower (MWh)
Y-Axis (Right): Monthly/annual precipitation levels (inches or mm)
Data: Plot energy production in regions with significant hydropower plants, like the Pacific Northwest, alongside precipitation data.
Insights: This graph could highlight how rainfall variability affects hydropower generation and how water resources impact energy availability.


**_6. Energy Consumption Growth vs. Climate Change Indicators (Temperature Rise, CO₂ Levels)_**

Graph Type: Line graph or area chart
X-Axis: Time (years or decades)
Y-Axis (Left): Total energy consumption (MWh)
Y-Axis (Right): Global CO₂ levels (ppm) or average global temperature anomaly (°C)
Data: Use long-term data for global CO₂ levels, temperature rise, and U.S. or regional energy consumption.
Insights: This graph visualizes the relationship between growing energy consumption and increasing climate change indicators, revealing how human energy use may be contributing to global warming.
