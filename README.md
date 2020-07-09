# R-Programming-Assigment-Week-4
This repo was created for the assignment due during week 4 of the Getting and Cleaning Data Coursera course.

The instructions involved the following - 
1. First, download and unzip the data file into your R working directory.
2. Second, download the R source code into your R working directory.
3. Finally, execute R source code to generate tidy data file.

Data description
The X variables in the data represent sensor signals measured using waist-mounted smartphones on 30 subjects, where as the Y variables reprsented the activity performed by each subject during the signal recording. 

Code explaination
The code required the creation of a new dataset which was a combination of the test and training datasets respectively. This data set extracted certain partial variables (mean and std) to create an independent new data set containing averages of each variable for each activity for all subjects. The code combined training dataset and test dataset, and extracted partial variables to create another dataset with the averages of each variable for each activity.

The code was written based on the instruction of this assignment.
- Read training and test dataset into R environment. Read variable names into R envrionment. Read subject index into R environment.
- Merges the training and the test sets to create one data set. Use command rbind to combine training and test set
- Extracts only the measurements on the mean and standard deviation for each measurement. Use grep command to get column indexes for variable name contains "mean()" or "std()"
- Uses descriptive activity names to name the activities in the data set Convert activity labels to characters and add a new column as factor
- Appropriately labels the data set with descriptive variable names. Give the selected descriptive names to variable columns
- From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject. Use pipeline command to create a new tidy dataset with command group_by and summarize_each in dplyr package

Three components of this assignment - 
CodeBook.md a code book that describes the variables, the data, and any transformations done to the data set. 
run_analysis.R contains the code done as per the 5 steps required by the assignment. 
FinalData.txt is the exported final data.
