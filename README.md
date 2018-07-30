# Getting and Cleaning data - Final assessment
This is the final assessment (week 4) for the course Getting and Cleaning data (Coursera - Data Scientist). 
Data is obtained from http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones# (Human Activity Recognition Using Smartphones Data Set). 

The repository contains the following files:
- CodeBook.md: A codebook that modifies and updates the available codebooks with the data to indicate all the variables and summaries calculated, along with units, and any other relevant information.
- run_analysis.R: Code is written in R by Stephanie Wassenburg, and does the following:
  - Download the dataset if it's not already in the working directory
  - Unzip the datafile
  - Read files
  - Merge the training and the test sets to create one data set
  - Extract only the measurements on the mean and standard deviation for each measurement
  - Use descriptive activity names to name the activities in the data set
  - Label the data set with descriptive variable names
  - Creates a second, independent tidy data set with the average of each variable for each activity and each subject
- FinalData.txt is the exported data file resulting from the last step in the code file.







