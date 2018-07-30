####Code Book

###Data Source
Data was obtained from http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones#
Please see the README and features.txt files in the original dataset to learn more about the original dataset and attribute information. 

###Data set
This Code Book modifies and updates the available codebooks with the data 
to indicate all the variables and summaries calculated, along with units, and any other relevant information.

- The dataset was downloaded and extracted under the folder called "UCI HAR Dataset".
- Each file was assigned to the following variables:
  - activities: activity_labels.txt with 561 rows and 2 columns. (List of activities)
  - features: features.txt with 6 rows and 2 columns. (List of all features)
  - subject_test: subject_test.txt with 2947 rows and 1 column. (Rows represent subjects 1-30 who performed the activity for each window sample)
  - x_test: X_test.txt with 2947 rows and 561 columns. (Test set)
  - y_test: y_test.txt with 2947 rows and 1 column. (Test labels)
  - subject_train: subject_train.txt with 7352 rows and 1 column. (Rows represent subjects 1-30 who performed the activity for each window sample)
  - x_train: X_train.txt with 7352 rows and 561 columns. (Training set)
  - y_train: y_train.txt with 7352 rows and 1 column. (Training labels)
  
###Transformation
In run_analysis.R, a tidy dataset is created following 5 steps as outlined by the assignment description.
1. Merges the training and the test sets to create one data set.
2. Extracts only the measurements on the mean and standard deviation for each measurement.
3. Uses descriptive activity names to name the activities in the data set
4. Appropriately labels the data set with descriptive activity names.
5. Creates a second, independent tidy data set with the average of each variable for each activity and each subject.

x_train and x_test were merged with rbind(): X (10299 rows, 561 columns)
y_train and y_test were merged with rbind(): Y (10299 rows, 1 column) 
subject_train and subject_test were merged with rbind(): Subject (10299 rows, 1 column) 
Subject, Y and X were merged with cbind(): Merged_Data (10299 rows, 563 column)

Means and Standard deviations for each measurement were selected for the columns 'subject' and 'code', resulting in TidyData.

Column names were changed in the following way:
Acc = Accelerometer
Gyro = Gyroscope
BodyBody = Body
Mag = Magnitude
start with 'f' = Frequency
start with 't' = Time
-mean() = Mean
-std() = Std
-freq() = Frequency

FinalData.txt (180 rows, 88 columns) was created by summarizing TidyData.
