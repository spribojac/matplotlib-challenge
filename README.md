<picture>
 <source media="(prefers-color-scheme: dark)" srcset="YOUR-DARKMODE-IMAGE">
 <source media="(prefers-color-scheme: light)" srcset="YOUR-LIGHTMODE-IMAGE">
</picture>

# MatPlotLib Challenge
## Module 5 MatPlotLib Challenge for University of Birmingham Data Analytics Bootcamp
### Description
-------------------------------------------------------------------------------------------------------------------------------------------------
### Pymaceuticals Challenge
------------------------------------------------------------------------------------------------------------------------------------------------

## Instructions
This assignment is broken down into the following tasks:
- Prepare the data.
- Generate summary statistics.
- Create bar charts and pie charts.
- Calculate quartiles, find outliers, and create a box plot.
- Create a line plot and a scatter plot.
- Calculate correlation and regression.
- Submit your final analysis.

### Prepare the Data
1. Run the provided package dependency and data imports, and then merge the mouse_metadata and study_results DataFrames into a single DataFrame.
2. Display the number of unique mice IDs in the data, and then check for any mouse ID with duplicate time points. Display the data associated with that mouse ID, and then create a new DataFrame where this data is removed. Use this cleaned DataFrame for the remaining steps.
3. Display the updated number of unique mice IDs.

### Generate Summary Statistics
Create a DataFrame of summary statistics. Remember, there is more than one method to produce the results you're after, so the method you use is less important than the result.
Your summary statistics should include:
1. A row for each drug regimen. These regimen names should be contained in the index column.
2. A column for each of the following statistics: mean, median, variance, standard deviation, and SEM of the tumor volume.

### Create Bar Charts and Pie Charts
Generate two bar charts. Both charts should be identical and show the total total number of rows (Mouse ID/Timepoints) for each drug regimen throughout the study.
1. Create the first bar chart with the Pandas DataFrame.plot() method.
2. Create the second bar chart with Matplotlib's pyplot methods.

Generate two pie charts. Both charts should be identical and show the distribution of female versus male mice in the study.

1. Create the first pie chart with the Pandas DataFrame.plot() method.
2. Create the second pie chart with Matplotlib's pyplot methods.

### Calculate Quartiles, Find Outliers, and Create a Box Plot
Calculate the final tumor volume of each mouse across four of the most promising treatment regimens: Capomulin, Ramicane, Infubinol, and Ceftamin. Then, calculate the quartiles and IQR, and determine if there are any potential outliers across all four treatment regimens. Use the following substeps:

1. Create a grouped DataFrame that shows the last (greatest) time point for each mouse. Merge this grouped DataFrame with the original cleaned DataFrame.
2. Create a list that holds the treatment names as well as a second, empty list to hold the tumor volume data.
3. Loop through each drug in the treatment list, locating the rows in the merged DataFrame that correspond to each treatment. Append the resulting final tumor volumes for each drug to the empty list.
4. Determine outliers by using the upper and lower bounds, and then print the results.

Using Matplotlib, generate a box plot that shows the distribution of the final tumor volume for all the mice in each treatment group. Highlight any potential outliers in the plot by changing their color and style.

hint: All four box plots should be within the same figure. Use this Matplotlib documentation pageLinks to an external site. for help with changing the style of the outliers.

### Create a Line Plot and a Scatter Plot
Select a single mouse that was treated with Capomulin, and generate a line plot of tumor volume versus time point for that mouse.

Generate a scatter plot of mouse weight versus average observed tumor volume for the entire Capomulin treatment regimen.

### Calculate Correlation and Regression
Calculate the correlation coefficient and linear regression model between mouse weight and average observed tumor volume for the entire Capomulin treatment regimen.

Plot the linear regression model on top of the previous scatter plot.

### Credits
-------------------------------------------------------------------------------------------------------------------------------------------------
Thank you to the bootcamp study groups. I built my logic around the exercises shared in class.
