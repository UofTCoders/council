# Week 1 (4 marks) Intro to programming
1. Why is it beneficial to use a programming language rather than a spreadsheet software for data analyses?
2. Get setup with Rstudio at home (or a lab computer after hours). Install R, Rstudio, and the necessary packages (tidyverse, rmarkdown). Use `install.packages(<package_name>)`. Load all the libraries you installed into your environment with `library(<package_name>)` and send us the output of running `sessionInfo()`.
3. What is Rmarkdown and why are we using it in this class? How do you execute a chunk of code in an Rmarkdown document?
4. Is there anything in particular you are excited about learning about theoretical ecological population models and about using R for data analyses and modelling?

# Week 2 (8 marks) Rmarkdown, assignment, functions, vectors, data frames
All the following should be done with Rmarkdown.

1. Assignment
    a. Assign the value `5` to the variable/object `a`.
    b. Assign the result of `10/3` to the variable `b`.
    c. Assign the product of `a` and `b` to `c`.
    d. Write a function that multiplies two numbers and returns the result. Use it to assign the product of `a` and `b` to `c`.
2. Vectors
    a. Create a vector `v` with all integers 1-30.
    b. Use `v` to create a new vector `v_square` with the square of element 3, 6, 7, 10, 15, 22, 23, 24, and 30 from `v`. Do _not_ use a for loop.
    c. Extract every 5th element from `v`, into a new vector `v_every_5th`.
4. Boolean indexing
    a. Create a boolean vector `v_bool` of the same length as `v`, indicating which vector elements are bigger than 20.
    b. Use `v_bool` as an index to extract the elements from `v` that are bigger than 20 and save as `v_over_20`.
    c. What's the mean of `v_over_20`?
5. Data frames
    a. What are the column names of inbuilt dataframe `iris`?
    b. How can you view the first 5 rows of this data frame?
    c. How many observations are there?
    d. Which factor levels are there? What is a factor level and when can it be useful?
    e. What is the mean value for the sepal.height column?
6. Save the data frame with only the species and sepal.width columns as csv-file. Load this csv file as a new data frame and run display its summary statistics.


# Week 3 (8 marks) dplyr, ggplot
All the following should be done with Rmarkdown.

```
# Setup
download.file("https://ndownloader.figshare.com/files/2292169",
              "data/portal_data_joined.csv")
surveys <- read.csv('data/portal_data_joined.csv')
```

1. Using two separate statements, select the columns `plot_id`, `species_id`, and `weight` from the `surveys` dataframe, and filter it to only include data from the year 1995. Do the same thing using pipes (%>%).
2. Create a new data frame from the surveys data that meets the following criteria: Contains only the species_id column and a new column called hindfoot_half containing values that are half the hindfoot_length values. In this  hindfoot_half column, there are no NAs and all values are less than 30.
3. Basic data aggregation.
    a. How many individuals were caught in each plot_type surveyed?
    b. Use group_by() and summarize() to find the mean, min, and max hindfoot length for each species (using species_id).
    c. What was the heaviest animal measured in each year? Return the columns  year, genus, species_id, and weight.
    d. Count the number of individuals of each sex.

4. Reshape data.
    a. Make a wide data frame with year as columns, plot_id as rows, and the values are the number of genera per plot. You will need to summarize before reshaping, and use the function n_distinct to get the number of unique types of a genera. It’s a powerful function! See ?n_distinct for more.
    b. Now take that data frame, and make it long again, so each row is a unique  plot_id year combination.
    c. The surveys data set is note truly wide or long because both there are two columns of measurement - hindfoot_length and weight. This makes it difficult to do things like look at the relationship between mean values of each measurement per year in different plot types. Let’s walk through a common solution for this type of problem. First, use gather to create a truly long dataset where we have a key column called measurement and a value column that takes on the value of either hindfoot_length or weight. Hint: You’ll need to specify which columns are being gathered.
    d. With this new truly long data set, calculate the average of each measurement in each year > for each different plot_type. Then spread them into a wide data set with a column for hindfoot_length and weight. Hint: Remember, you only need to specify the key and value columns for spread.
5. Plotting
    a. Make a histogram of the hindfoot length for year 1995.
    b. Make a scatter plot of the hindfoot length vs the weight.
    c. Color the data points in the scatter plot from 'b' by year and replace the circles with triangles.
    d. Give data points a light transparency and change the grey background to white.

