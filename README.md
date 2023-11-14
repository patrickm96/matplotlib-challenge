# matplotlib-challenge

Module 5

Final code for module 5 challenge is in pymaceuticals_analysis.ipynb.

The following resources were referenced in order to complete this challenge:

1. Import Modules - Starter code
2. Find duplicates in DataFrame based on subset - https://www.geeksforgeeks.org/python-pandas-dataframe-duplicated/#
3. Filter DataFrame based on column value - https://www.geeksforgeeks.org/ways-to-filter-pandas-dataframe-by-column-values/
4. Create PyPlot bar chart - https://www.w3schools.com/python/matplotlib_bars.asp
5. Add percentage value to Pandas pie chart - https://www.geeksforgeeks.org/how-to-create-pie-chart-from-pandas-dataframe/
6. Format outliers/flierprops - https://stackoverflow.com/questions/65648502/how-to-change-outlier-point-symbol-in-python-matplotlib-pyplot
7. Pandas bar plot - https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.plot.bar.html
8. PyPlot bar plot - https://www.geeksforgeeks.org/bar-plot-in-matplotlib/
9. Rotate axis tick labels - https://stackoverflow.com/questions/10998621/rotate-axis-tick-labels
10. Create PyPlot charts from np.array - https://www.geeksforgeeks.org/plot-line-graph-from-numpy-array/
11. Pandas pie chart - https://www.geeksforgeeks.org/how-to-create-pie-chart-from-pandas-dataframe/
12. Show PyPlot pie chart percentage - https://www.tutorialspoint.com/in-matplotlib-show-the-percentage-or-proportional-data-where-each-slice-of-pie-represents-a-category
13. Filter loc subset based on list values - https://deallen7.medium.com/using-pandas-loc-and-isin-to-filter-for-a-list-of-values-in-python-a1c862054058
14. Merge DataFrames on multiple columns - https://sparkbyexamples.com/pandas/pandas-merge-two-dataframes-on-multiple-columns/?expand_article=1
15. Rename xticks in matplotlib boxplot - https://stats.stackexchange.com/questions/3476/how-to-name-the-ticks-in-a-python-matplotlib-boxplot
16. DataFrame aggregate functions - https://www.w3resource.com/pandas/dataframe/dataframe-agg.php
17. Quartiles - Instructor Eli Rosenberg covered this during class.
18. Format graphs - Instructor Eli Rosenberg covered this during class.
19. Create scatter plot - Instructor Eli Rosenberg covered this during class.
20. Correlation, regression & line equation calculation and graphs - Instructor Eli Rosenberg covered this during class.

## Instructions
This assignment is broken down into the following tasks:

Prepare the data.
Generate summary statistics.
Create bar charts and pie charts.
Calculate quartiles, find outliers, and create a box plot.
Create a line plot and a scatter plot.
Calculate correlation and regression.
Submit your final analysis.

### Prepare the Data
Run the provided package dependency and data imports, and then merge the mouse_metadata and study_results DataFrames into a single DataFrame.

Display the number of unique mice IDs in the data, and then check for any mouse ID with duplicate time points. Display the data associated with that mouse ID, and then create a new DataFrame where this data is removed. Use this cleaned DataFrame for the remaining steps.

Display the updated number of unique mice IDs.

### Generate Summary Statistics
Create a DataFrame of summary statistics. Remember, there is more than one method to produce the results you're after, so the method you use is less important than the result.

Your summary statistics should include:

A row for each drug regimen. These regimen names should be contained in the index column.
A column for each of the following statistics: mean, median, variance, standard deviation, and SEM of the tumor volume.

### Create Bar Charts and Pie Charts
Generate two bar charts. Both charts should be identical and show the total total number of rows (Mouse ID/Timepoints) for each drug regimen throughout the study.

Create the first bar chart with the Pandas DataFrame.plot() method.

Create the second bar chart with Matplotlib's pyplot methods.

Generate two pie charts. Both charts should be identical and show the distribution of female versus male mice in the study.

Create the first pie chart with the Pandas DataFrame.plot() method.

Create the second pie chart with Matplotlib's pyplot methods.

### Calculate Quartiles, Find Outliers, and Create a Box Plot
Calculate the final tumor volume of each mouse across four of the most promising treatment regimens: Capomulin, Ramicane, Infubinol, and Ceftamin. Then, calculate the quartiles and IQR, and determine if there are any potential outliers across all four treatment regimens. Use the following substeps:

Create a grouped DataFrame that shows the last (greatest) time point for each mouse. Merge this grouped DataFrame with the original cleaned DataFrame.

Create a list that holds the treatment names as well as a second, empty list to hold the tumor volume data.

Loop through each drug in the treatment list, locating the rows in the merged DataFrame that correspond to each treatment. Append the resulting final tumor volumes for each drug to the empty list.

Determine outliers by using the upper and lower bounds, and then print the results.

Using Matplotlib, generate a box plot that shows the distribution of the final tumor volume for all the mice in each treatment group. Highlight any potential outliers in the plot by changing their color and style.

hint: All four box plots should be within the same figure. Use this Matplotlib documentation pageLinks to an external site. for help with changing the style of the outliers.

### Create a Line Plot and a Scatter Plot
Select a single mouse that was treated with Capomulin, and generate a line plot of tumor volume versus time point for that mouse.

Generate a scatter plot of mouse weight versus average observed tumor volume for the entire Capomulin treatment regimen.

### Calculate Correlation and Regression
Calculate the correlation coefficient and linear regression model between mouse weight and average observed tumor volume for the entire Capomulin treatment regimen.

Plot the linear regression model on top of the previous scatter plot.
