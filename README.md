🚲 Bike Sharing Demand Analysis – Hourly & Daily Trends
📌 Overview
This project explores and analyzes the bike sharing dataset collected on an hourly and daily basis in Washington, D.C. The goal is to understand how different factors such as weather, time of day, season, and holidays influence the demand for bike rentals, both by casual users and registered users.

🗂️ Dataset
Source: UCI Machine Learning Repository – Bike Sharing Dataset

Files Used:

hour.csv – Hourly bike rental data

day.csv – Daily bike rental data

🛠️ Tools & Libraries Used
Language: R

Libraries:

tidyverse, dplyr, ggplot2 – Data wrangling and visualization

plotly, gridExtra, beanplot – Advanced visualizations

gplots, RColorBrewer – Enhanced plotting

knitr – Report formatting

🔍 Key Tasks Performed
1. 📦 Data Import & Cleaning
Removed the instant column as it's just an index.

Converted relevant variables to factors (e.g., season, weather, holiday).

Renamed factor levels to meaningful labels (e.g., 1 to Spring).

Identified and removed outliers using IQR (for both casual and registered users).

Analyzed zero-value records for insights on non-usage periods.

2. 📈 Feature Engineering
Created Ratio of registered to casual users to understand usage dynamics.

Categorized hours into time-of-day segments: Morning, Afternoon, Evening, and Night.

3. 📊 Exploratory Data Analysis (EDA)
Hourly trend analysis across days of the week and hours.

Comparison of casual vs. registered usage by:

Month

Season

Weather

Holidays

Used boxplots, beanplots, and grouped bar plots to visualize relationships.

Generated PDF plots to understand the distribution of rentals.

4. 📉 Correlation & Regression
Conducted correlation tests between temperature (atemp) and rental count (cnt) for both years.

Plotted regression lines to observe trends over time.

📌 Visual Insights
Clear weather and spring/fall seasons see higher usage.

Registered users dominate during weekdays, while casual users peak on weekends.

Holiday vs. Non-Holiday behavior shows distinct rental patterns.

Positive correlation between apparent temperature and rental demand.
