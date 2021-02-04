# Matplotlib Challenge

## Background

For this challenge I was given access to the complete data from Pymaceuticals' most recent animal study. In this study, 249 mice identified with SCC tumor growth were treated through a variety of drug regimens. Over the course of 45 days, tumor development was observed and measured. The purpose of this study was to compare the performance of Pymaceuticals' drug of interest, Capomulin, versus the other treatment regimens. You have been tasked by the executive team to generate all of the tables and figures needed for the technical report of the study. The executive team also has asked for a top-level summary of the study results.

This data can be found here at Pymaceuticals/data

## Observations & Insights
* Capomulin and Ramicane resulted in much smaller tumor volume at the end of their mice's timepoint's when compared with the other drugs. Suggesting that these drugs might be the most efficient
* Infubinol appears to have an outlier that should be thrown out or investigated.
* There seems to be a rather strong correlation between tumor volume and mouse weight which intuitively makes sense.

## Data Analysis

The code and results of the following can be found here at Pymaceuticals/pymaceuticals.ipynb

* Cleaned the data by merging the two csv files into one DataFrame and and removing any duplicate timepoints.

* Generated a summary statistics table consisting of the mean, median, variance, standard deviation, and SEM of the tumor volume for each drug regimen.

* Generated a bar plot using both Pandas's `DataFrame.plot()` and Matplotlib's `pyplot` tho show the total number of measurements taken for each treatment regimen throughout the course of the study.

* Generated a pie plot using both Pandas's `DataFrame.plot()` and Matplotlib's `pyplot` tho show the distribution of female or male mice in the study.

* Calculated the final tumor volume of each mouse across four of the most promising treatment regimens: Capomulin, Ramicane, Infubinol, and Ceftamin. Calculated the quartiles and IQR and quantitatively determined if there are any potential outliers across all four treatment regimens.

* Utilized Matplotlib to generate a box and whisker plot of the final tumor volume for all four treatment regimens to identify any potential outliers.

* Selected a mouse that was treated with Capomulin and generated a line plot of tumor volume vs. time point for that mouse.

* Generated a scatter plot of mouse weight versus average tumor volume for the Capomulin treatment regimen.

* Calculated the correlation coefficient and linear regression model between mouse weight and average tumor volume for the Capomulin treatment. Plotted the linear regression model on top of the previous scatter plot.

