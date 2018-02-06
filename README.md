# Getting-and-Cleaning-Data-Assignment
This is a summary for the assignment of Getting and Cleaning Data Course Project. Using R-studio (Version 1.1.383).

Step 1. 
The following files was downloaded from project assignment page into local drive.  

- 'features_info.txt': Shows information about the variables used on the feature vector.
- 'features.txt' - using read.delim function
- 'activity_labels.txt': Links the class labels with their activity name.
- 'train/X_train.txt': Training set.
- 'train/y_train.txt': Training labels.
- 'test/X_test.txt': Test set.
- 'test/y_test.txt': Test labels.

Step 2. The datasets were loaded into R- studio.  Test data sets (subject, activity label and results) were combined into 1 dataset, 
followed by combining train data sets into 1 dataset. Then the 2 datasets were combined into 1 data set with all the subjects, activity label and results. Column names were assigned using data from "features.txt" file.

Step 3. The mean and standard deviation columns were extracted into a new table, then activity names were incorporated into the dataset using "mapvalues" function. 

Step 4. Using "aggregate" function to generate a new dataset with the average of each variable for each activity and each subject.

##########################################

Brief information about the Human Activity Recognition Using Smartphones Dataset (Version 1.0)

created by:
Jorge L. Reyes-Ortiz, Davide Anguita, Alessandro Ghio, Luca Oneto.
Smartlab - Non Linear Complex Systems Laboratory
DITEN - Università degli Studi di Genova.
Via Opera Pia 11A, I-16145, Genoa, Italy.
activityrecognition@smartlab.ws
www.smartlab.ws

The experiments have been carried out with a group of 30 volunteers within an age bracket of 19-48 years. Each person performed six activities (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING) wearing a smartphone (Samsung Galaxy S II) on the waist. Using its embedded accelerometer and gyroscope, we captured 3-axial linear acceleration and 3-axial angular velocity at a constant rate of 50Hz. The experiments have been video-recorded to label the data manually. The obtained dataset has been randomly partitioned into two sets, where 70% of the volunteers was selected for generating the training data and 30% the test data. 

The sensor signals (accelerometer and gyroscope) were pre-processed by applying noise filters and then sampled in fixed-width sliding windows of 2.56 sec and 50% overlap (128 readings/window). The sensor acceleration signal, which has gravitational and body motion components, was separated using a Butterworth low-pass filter into body acceleration and gravity. The gravitational force is assumed to have only low frequency components, therefore a filter with 0.3 Hz cutoff frequency was used. From each window, a vector of features was obtained by calculating variables from the time and frequency domain. See 'features_info.txt' for more details. 
