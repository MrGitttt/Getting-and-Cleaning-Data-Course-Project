The run_analysis.R script performs the data preparation and then followed by the 5 steps required as described in the course project’s definition.

1. Merges the training and the test sets to create one data set
Using rbind() and cbind() to merge the data sets.

2. Extracts only the measurements on the mean and standard deviation for each measurement
TidyData is created by subsetting Merged_Data.

3. Uses descriptive activity names to name the activities in the data set
Entire numbers in code column of the TidyData replaced with corresponding activity taken from second column of the activities variable

4. Appropriately labels the data set with descriptive variable names
Using names() to rename the variables.

5. From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject
FinalData is created and exported after groupped by subject and activity based on dplyr.
