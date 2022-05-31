# Showcasing the process of how Mapper and Reducer functions work in Hadoop

## DATA DESCRIPTION
The provided txt file consists of 1000 lines of data which includes 2000 pairs of Year/month and the average temperature of that month. 


## GOAL
Goal is to find the maximum temperature for each year in provided txt file

## STEPS
Several steps are necessary to showcase how Mapper and Reducer functions work in Hadoop. These include:

* Step 1 (Data Cleaning): This includes removing punctuations and special symbols as well as converting string to integer. This is necessary to calculate the maximum temparture for each year.

* Step 2 (Data Split Function): Splitting the dataset into two parts. Part1 will include the first 500 lines of the raw txt file and Part2 will include the other 500 lines. 

* Step 3 (Mapper Function): Creating two mapper functions that produce a set of key-value pairs for Part1 and Part2 subsets respectively. 

* Step 4 (Sort Function): Sorting by key of Part1 and Part2 together with an ascending sort order

* Step 5 (Partition Function): All the months in year 2010 to 2015 are sent to Reducer1, and 2016 to 2020 are sent to Reducer2

* Step 6 (Reducer Funtion): Collecting all values belonging to the key and finding the maximum temeprature for the two ordered partitions.

* Step 7 (Main Function): Combining the output of the two partitions together

## RESULTS
The mapper and reducer functions worked perfectly and I was able to find the maximum temperatures of each year. Unfortunately, all of the maximum temperatures in the provided data resulted in 120. This is a limitation of the provided data. Overall, this showcased how mapper and reducer functions work in Hadoop.
