# getting cleaning data week 4 project

This project is conformed of 3 files of analysis:

getdata_projectfiles_UCI HAR Dataset: Is the raw dataset used to make the file tidyData.txt. It contains all neccesary files (train and test) to load and transform data required for this project.


run_analysis: Is the script used to transform the original files given for this project to finally obtain a tidy dataset following the project's indications:
- Merges the training and the test sets to create one data set.
- Extracts only the measurements on the mean and standard deviation for each measurement.
- Uses descriptive activity names to name the activities in the data set
- Appropriately labels the data set with descriptive variable names.
- From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.


Codebook:

trainingData: Create the final training set by merging yTrain, subjectTrain, and xTrain

testData: final test set by merging the xTest, yTest and subjectTest data

colNames:  a vector for the column names from the finalData, which is used to select the desired mean() & stddev() columns

logicalVector: logicalVector that contains TRUE values for the ID, mean() & stddev() columns and FALSE for others

finalData: Subset finalData table based on the logicalVector to keep only desired columns containing training and test data

finalDataNoActivityType: new table without the activityType column

tidyData : table to include just the mean of each variable for each activity and each subject
