# cleaning_data
Cleaning data

The script loads both the train and test sets into the workspace environment 
Features are loaded from the features.txt file, names in the features file(headers) are converted 
to valid R header names with periods removed. 

The test and train data are merged using dplyr's bind_rows function and then he headers of the resulting
data set is set to the features vector.

#2 
The measuremenst on the mean and standard deviation for each measurement are extracted using select and the matches helper function. 

#3
A activity column was created to show the different activities performed for each observation and descriptive activity names were used to replace the integer-coded representation.

#5
A grouping of the data, based on activity, was done and the mean of each of the columns calculated using summarise_all and the mean function.
The same would be done for the subjects. The subjects data should be loaded as a vector, joined to the existing data set, with a header named 'subject' and a grouping should be done based on subject and finally a summarise_all with a call to the mean function.

