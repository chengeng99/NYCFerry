# NYCFerry
This repository includes dataset, Rmd, and a brief instruction on how to rerun the data analysis.

To rerun my analysis for NYC Ferry Ridership, follow these steps:
1. Create a new R project and a new R or R Markdown file within the project you created

2. Install Required Libraries: Make sure you have the required R libraries - tidyverse, fs, and
RColorBrewer installed before running other commands

3. Download and Import Data: Download the NYC Ferry Ridership dataset from NYC Open Data
and save it as "NYC_Ferry_Ridership.csv" in your R project. Then, run the code to import the
dataset into R; dataset link here: https://data.cityofnewyork.us/Transportation/NYC-Ferry-Ridership/t5n6-gx8c/data

4. Prepare Data for Analysis: The dataset contains information for weekdays and weekends.
As the research focuses on weekday peak hours, filter out weekends from the dataset

5. Aggregate Peak-Hour Ridership: Calculate the average hourly ridership during morning (6-10
am) and evening (4-7 pm) peak hours for each weekday

6. Create Trend Line Plots: Plot the trend of average hourly ridership during morning and
evening peak hours over the six-year period using the geom_smooth and geom_vline in
ggplot library (it comes with tidyverse)

7. Filter and Visualize Individual Route Trends: Analyze the trend of ridership during AM and
PM rush hours for each individual NYC Ferry route using geom_smooth and geom_vline

8. Directional Pattern Analysis: Analyze the directional pattern of each ferry route during
morning and evening peak hours using stacked-bar plots (geom_bar)

9. Save the visualizations using the Export function in R: save as PDF with size 7’’ * 5.28’’
