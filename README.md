# Exploratory Data Analysis of MTA Turnstile Data
## **Abstract**

The goal of this project was to find the specific places in the New York City area that my client, street performer and violinist Karolina Protsenko, should perform in order to maximize the amount of foot traffic that would see her performances. I used turnstile data from the Metropolitan Transit Authority (MTA) in October - December 2021 in order to determine the stations and times of day with the most people entering and exiting. I used the Python library Plotly to visualize and communicate the results through interactive line plots and a geographic map.

## **Design**

[Karolina Protsenko](https://www.youtube.com/watch?v=7tQIJMXIG1Q) is a street performer and violinist. She is interested to know where exactly she should perform in NYC such that she reaches the largest audience possible. Exploratory data analysis on MTA turnstile data would provide insights on the most populated locations, days of the week, and times of the day for Karolina to perform.

## **Data**

The dataset contains cumulative turns per turnstile for all MTA stations over the course of 91 days. Turnstile identification, station, date, time, entries, and exits are included. Most turnstiles were measured every four hours, though there were many exceptions. Entries and exits were combined in analysis, as this client is concerned with total traffic in a particular area of the city. Times were important in order to inform the client what times of day are most crowded. The most recent three months of data, October through December 2021, were included because this client is interested in performing soon, and historical data may not provide accurate predictions for today due to differing traffic patterns throughout the pandemic. 

## **Algorithms**

A thorough exploratory data analysis was performed of MTA turnstile data. Cumulative turnstile entries and exits were used to calculate the total number of people entering and exiting the station in a given duration of time. Each station contains many turnstiles, so all turnstiles for a given station were combined to produce a value for the entire station. Stations were then ranked according to the total number of people entering and exiting to provide the most populated stations. The total foot traffic in the five most populated stations were plotted as a function of time over the course of a day to indicate the times of day with the most traffic.

## **Tools**

- DB Browser for SQLite for extracting and transforming raw data
- SQLAlchemy for querying database into Python
- Pandas for data manipulation, cleaning, and analysis
- Matplotlib for plotting
- Plotly for interactive visualizations
- RISE for presenting

## **Communication**

[RISE](https://rise.readthedocs.io/en/stable/index.html#), a Jupyter Notebook slideshow extension, was used to present slides and interactive visuals.
