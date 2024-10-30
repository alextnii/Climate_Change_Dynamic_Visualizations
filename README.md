# Climate_Change_Dynamic_Visualizations
Created Several Interactive Data Visualizations for Environmental Power Research Institute (EPRI) Contract

## General Background 
Electric Power Research Institute (EPRI) is a leading research organization dedicated to advancing the reliable, affordable, and resilient future of energy. EPRI is known for its unbiased, science-driven approach, rigorously focusing on objective research to guide the energy industry without advocating for specific companies, sectors, or technologies. Their mission is to deliver independent thought leadership and practical insights that benefit society at large, empowering the energy sector through collaborative and data-driven solutions.

I am currently a Project Manager at DataStory, a data science consulting organization at UC Berkeley. Initially contracted as part of a semester-long consulting project, I transitioned from being a consultant/programmer to assuming a more central role as Project Manager toward the end of the engagement. This transition gave me the opportunity to not only contribute to the technical aspects of the project but also manage our team toward the end.

## Project Overview

The primary objective of this project was to leverage data analysis and visualization techniques to derive meaningful insights from complex energy-related datasets provided by EPRI. As a part of EPRI's mission to foster innovation in the energy industry, the datasets contained valuable information regarding energy usage patterns, weather data, and climate variables that could influence energy distribution and consumption.

The project's goals can be summarized as follows:
1. Data Cleaning and Preprocessing: The first step involved extracting relevant data from raw files and performing necessary transformations. This included:
- Handling missing or corrupt data entries.
- Aggregating data by time intervals (e.g., year, month) for better visualization.
- Converting energy and temperature units to standardized formats.

2. Interactive Visualizations: The next phase focused on creating dynamic, interactive visualizations to help EPRI's analysts as well as users on their webpage to explore the data more intuitively. Key visualizations included:
- Line charts showing temperature trends over time for different cities.
Box plots that presented temperature variations by month or year, highlighting extreme values.
- Histograms for the distribution of maximum and minimum temperatures.
- Map-based visualizations that utilized geographical data to map energy patterns against weather conditions.

## Data and Methodology
1. Data Sources
- Temperature Data: The dataset included daily maximum and minimum temperatures (tmax and tmin) across multiple cities, spanning several decades. This was essential to understanding how climate variables have impacted energy consumption over time.
- Energy Usage Logs: These logs detailed the energy distribution and usage patterns across different regions. This data was crucial for cross-referencing with weather information to study the relationship between temperature fluctuations and energy demand.
2. Data Cleaning and Processing
The raw data was structured into separate files and needed significant preprocessing. Below are some key steps in this process:
- Handling Missing Data: Certain regions had missing entries for both temperature and energy usage logs. We employed imputation techniques and interpolation to estimate missing values without compromising the data integrity.
- Data Aggregation: To simplify the analysis, we aggregated data on a monthly and yearly basis. This allowed us to identify long-term trends without getting lost in the noise of day-to-day fluctuations.
- Unit Conversion: Temperature data was originally recorded in Celsius, which we converted to Fahrenheit to better align with energy reports typically used in the U.S.
3. Visualization and Analysis
Bokeh and Panel were employed for creating interactive visualizations, allowing users to manipulate the data on the fly. Key visualizations included:
- Temperature Box Plots: This visualization allowed users to compare the maximum and minimum temperatures across cities and see how they varied by month or year. The interactivity made it easy for users to filter cities and time periods and adjust the granularity of the data.
- Line Charts: These charts illustrated temperature trends over time, making it easier to visualize the correlation between rising temperatures and increasing energy demands.
- Histograms: By analyzing the distribution of temperature data, the histograms helped to identify frequent temperature ranges, which could be used to predict typical energy needs.
- Geospatial Visualizations: Using geographical data (latitude and longitude), we built maps to overlay temperature data with energy usage, allowing EPRI stakeholders to explore regional variations in energy consumption.

## Tools and Technologies
- Python Libraries: For data manipulation, we relied on popular Python libraries such as Pandas for handling large datasets, Xarray for working with multidimensional arrays (e.g., temperature data), and NumPy for numerical calculations.
- Panel and Bokeh: These were the core libraries used for creating the interactive dashboard. Panel enabled the creation of dynamic, server-ready applications, while Bokeh provided robust plotting capabilities.
- Plotly: In addition to Bokeh, Plotly was used for more complex visualizations, such as the box plots and histograms, which benefited from Plotly’s flexible layout options.
- Jupyter Notebooks: The entire workflow was initially developed and tested in Jupyter notebooks, allowing for rapid prototyping and easy collaboration with the rest of the team.

## Project Reflection
From a personal perspective, this project was not only a learning experience in terms of technical skills but also an opportunity to grow in a leadership role.
