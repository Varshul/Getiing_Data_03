Getting_Data_03
===============
A few steps were taken to transform the initial data set. The test and train sets have were merged and the subject identifiers and activity labels were pulled in to create a single data set. The activity identifiers were translated from identifiers into human-readable names. Only the mean and standard deviation variables were kept. Those variables were further summarized by taking their mean for each subject/activity pair. There is a single row for each subject/activity pair, and a single column for each measurement.

The final data set can be found in the tidy_set.txt file, which can be read into R with read.table("tidy_set.txt", header = TRUE). 
