Coursera - Getting and cleaning data: Project
===========

## Introduction

(From the course project webpage)

One of the most exciting areas in all of data science right now is wearable computing - see for example this article: http://www.insideactivitytracking.com/data-science-activity-tracking-and-the-battle-for-the-worlds-top-sports-brand/ . Companies like Fitbit, Nike, and Jawbone Up are racing to develop the most advanced algorithms to attract new users. The data linked to from the course website represent data collected from the accelerometers from the Samsung Galaxy S smartphone. A full description is available at the site where the data was obtained: 

http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones 

Here are the data for the project: 

https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip 

## Objective

(From the course project webpage)

Create one R script called *run_analysis.R* that does the following. 

1. Merges the training and the test sets to create one data set.

2. Extracts only the measurements on the mean and standard deviation for each measurement. 

3. Uses descriptive activity names to name the activities in the data set

4. Appropriately labels the data set with descriptive variable names. 
5. From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.


## Files of the study

* *README.md*: This file.
* *Codebook.md*: The codebook with the information about the tidy dataset and the summary data set.
* *run_analysis.R*: The script with the steps to process the raw data into the tidy dataset and the summary data set.


## Technical information

### Tests
The script *run_analysis.R* was executed more than once to confirm it generates the same result each time.

### Tool versions
The script was written and executed using RStudio 0.99.465 with R 3.2.1 installed.
The machine used to write and execute the script is using Windows 8.1 64bits.

### Library dependencies
The script uses the following R libraries:

* data.table
* plyr
* dplyr 


## Instruction list

In order to generate the tidy datasets:

1. Step 1: Run the script *run_analysis.R* in R version 3.2.1 or newer.

2. Step 2: After the execution, in R (or R studio) you can use the tidy data set by using the object *mergedDataset*.

3. Step 3: On the */data/* subdirectory of the working directory you will find the summary data set in the file *Summary UCI HAR Dataset - Average values by subject and activity.txt* .


## Explanation of the script

The script *run_analysis.R* does the following:

1. Create the subdirectory */data/* if it doesn't exists,

2. Download the raw data files from the URL mentioned on the *Introduction* section, if they aren't already downloaded.

3. Read the labels for features and activities

4. Read and merge the test and training sets of subjects, measurements and activities

5. Select only the measurements for the mean and standard deviation. In this step, the meanFreq() measurements (as explained on the features_info.txt file of the original experiment) are not included here because the nature of those values is out of the current project scope. 

6. Rename the variables for measurements with more descriptive names. At this step, the mergedDataset object is generated in R and can be used after the execution of the script (as described on step 2 of the *Instruction list* section)

7. Generate the summary data set and write the output to the file *Summary UCI HAR Dataset - Average values by subject and activity.txt* into the working directory.
