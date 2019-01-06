# Scotland Whiskey Analysis 2017 

## A co-relation between multiple qualities of whiskey samples collected from distilleries in Scotland


The generated graph will then be plotted along a geographic plot.

### Step-1

#### Import the necessary libraries

pandas - Database management
numpy - Optimized Numerical Calculations
sklearn - Data Science libraries
bokeh, matplotlib - plotting graphs

### Step-2

#### Define important file names

These filenames will be required later in the code

**"n_classes"** stores the number of classifications of whiskey
**"flavor_index"** stores the index numbers of the flavors

### Step-3

#### Load the databases and combine them into one

The new database is now stored in "whiskies_with_regions.txt"

We do so using the pandas library.


### Step-4

#### Generate the correlation matrix

#### What is a Correlation Matrix?

A correlation matrix is a table showing correlation coefficients between sets of variables. Each random variable (Xi) in the table is correlated with each of the other values in the table (Xj). This allows you to see which pairs have the highest correlation.

![image](https://i.ibb.co/YpNhjFv/Screenshot-from-2019-01-06-20-42-09.png)

### Step-5

#### Arrange the generated matrix

We try to cluster the distillaries into "n_classes" groups based on similar features of whiskies produced by them. Then we arrange the matrix in such a way that those clusters are placed together, showing visible "n_classes" regions along the diagonal in the generated plot.

![image](https://i.ibb.co/qR9wr19/Screenshot-from-2019-01-06-20-41-27.png)

### Step-6

#### Plot the clustered-correlations clearly in an interactive plot

We'll be using Bokeh library for plotting the interactive graph

First we assign random colors to each cluster

We use bokeh to plot the same graph in a clearer and interative way

![image](https://i.ibb.co/njymMJC/distillery-type-cluster.png)

### Step-7

#### Plot an interactive geographic plot based on one specfied parameter

We'll be using the "Group" or cluster as the default parameter of coloring.

First, assign random colors to each category.

Plot the interactive geographic plot using bokeh library.

![image](https://i.ibb.co/pnWMMwd/distillery-type-demographic.png)