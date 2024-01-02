# data-visualization
For this assignment, the first part was preparing the data.
I began by importing the dependencies and doing some initial setup.
I created paths for and read in the two data files, then combined them into a single dataframe and displayed this new data table.
Next, I checked the number of mice.
Then I checked for any duplicate mice by ID number that would show up for Mouse ID and Timepoint.
I then created a table to display the data for the duplicate mouse ID.
I created a new, clean dataframe by removing the duplicate mouse by its ID, then checked the number of mice in the clean dataframe.
The next part focused on generating summary statistics.
I used groupby and summary statistical methods to calculate the mean, median, variance, standard deviation, and standard error of mean (SEM) of the tumor volume for each drug regimen, then I generated a summary statistics table of these values and assembled them into a single summary dataframe.
I did the same thing again but using the aggregation method, which produced the same statistics in a single line.
The following part called for creating bar charts and pie charts.
I created a count for the number of instances for each drug regimen.
The first bar chart displayed the number of observed mouse timepoints for each drug regimen by using Pandas.
The second bar chart displayed the number of observed mouse timepoints for each drug regimen by using pyplot.
The first pie chart displayed the distribution of female versus male mice using Pandas.
The second pie chart displayed the distribution of female versus male mice using pyplot.
The next section was based on quartiles, outliers, and box plots.
I calculated the final tumor volume of each mouse across four of the treatment regimens:  Capomulin, Ramicane, Infubinol, and Ceftamin.
I started by getting the last (greatest) timepoint for each mouse, then merged this group dataframe with the original dataframe to get the tumor volume at the last timepoint.
I set up a list for the treatments for the for loop, and later for plot labels, and created an empty list to fill with tumor volume data for plotting.
I created a for loop that located the rows which contain mice on each drug and got the tumor volumes, then added the subset.
I then set the quartiles, set a lower quartile and upper quartile, calculated the IQR, lower bound, upper bound, and any outliers, printing a statement for each drug regimen.
With all these values, I generated a box plot that shows the distrubution of the tumor volume for each treatment group.
The next section's purpose was to create line and scatter plots.
The line plot displayed tumor volume vs time point for a single mouse treated with Capomulin.
The scatter plot showed mouse weight vs the average observed tumor volume for the entire Capomulin regimen
The last section calculated correlation and regression.
I calculated the correlation coefficient for mouse weight and average observed tumor volume for the entire Capomulin regimen, then printed a statement that gave the correlation value.
Lastly, I calculated the linear regression model and displayed it on top of the previous scatter plot that showed the relationship between weight and average tumor volume.
