Study design
===========
The raw data was gathered from coursera's course project page. 
The information about the original experiment, source for this tidy dataset, can be found on http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones
Into the zip file containing the dataset, the reference files to understand the experiment are:

* README.txt: Gives general information about the experiment.
* features_info.txt: Describes how the values were obtained and computed.
* features.txt: The list of the variable names used on the raw data.
* activity_labels.txt: The list of values/description for the activity variable.

Code book
===========

### Tidy data

The tidy data computed by the script run_analysis.R includes all the mean and standard deviations measurements from the original experiment, for both test and training datasets. Please note that the meanFreq() measurements (as explained on the features_info.txt file of the original experiment) are not included here because the nature of those values is out of the current project scope. 
Each row corresponds to a unique observation and includes the following variables:

* ID_subject: Value between 1 and 30. Identifies the subject of the measurements
* measurement_type: "TEST" or "TRAINING". Identifies the measurement type of the row
* ID_activity: value between 1 and 6. Identifies the activity measured and corresponds to the variable "activity"
* activity: Description of the variable ID_activity: 
    + For ID_activity 1 = "WALKING"
    + For ID_activity 2 = "WALKING_UPSTAIRS"
    + For ID_activity 3 = "WALKING_DOWNSTAIRS"
    + For ID_activity 4 = "SITTING"
    + For ID_activity 5 = "STANDING"
    + For ID_activity 6 = "LAYING"
* bodyAccelerationMeanByTime_XAxis: Value between -1 and 1. Mean body acceleration gathered from the accelerometer (X axis) in the time domain.
* bodyAccelerationMeanByTime_YAxis: Value between -1 and 1. Mean body acceleration gathered from the accelerometer (Y axis) in the time domain.
* bodyAccelerationMeanByTime_ZAxis: Value between -1 and 1. Mean body acceleration gathered from the accelerometer (Z axis) in the time domain.
* gravityAccelerationMeanByTime_XAxis: Value between -1 and 1. Mean gravity acceleration gathered from the accelerometer (X axis) in the time domain.
* gravityAccelerationMeanByTime_YAxis: Value between -1 and 1. Mean gravity acceleration gathered from the accelerometer (Y axis) in the time domain.
* gravityAccelerationMeanByTime_ZAxis: Value between -1 and 1. Mean gravity acceleration gathered from the accelerometer (Z axis) in the time domain.
* bodyAccelerationJerkMeanByTime_XAxis: Value between -1 and 1. Mean Jerk body acceleration gathered from the accelerometer (X axis) in the time domain.
* bodyAccelerationJerkMeanByTime_YAxis: Value between -1 and 1. Mean Jerk body acceleration gathered from the accelerometer (Y axis) in the time domain.
* bodyAccelerationJerkMeanByTime_ZAxis: Value between -1 and 1. Mean Jerk body acceleration gathered from the accelerometer (Z axis) in the time domain.
* bodyAngularVelocityMeanByTime_XAxis: Value between -1 and 1. Mean body angular velocity gathered from the gyroscope (X axis) in the time domain.
* bodyAngularVelocityMeanByTime_YAxis: Value between -1 and 1. Mean body angular velocity gathered from the gyroscope (Y axis) in the time domain.
* bodyAngularVelocityMeanByTime_ZAxis: Value between -1 and 1. Mean body angular velocity gathered from the gyroscope (Z axis) in the time domain.
* bodyAngularVelocityJerkMeanByTime_XAxis: Value between -1 and 1. Mean Jerk body angular velocity gathered from the gyroscope (X axis) in the time domain.
* bodyAngularVelocityJerkMeanByTime_YAxis: Value between -1 and 1. Mean Jerk body angular velocity gathered from the gyroscope (Y axis) in the time domain.
* bodyAngularVelocityJerkMeanByTime_ZAxis: Value between -1 and 1. Mean Jerk body angular velocity gathered from the gyroscope (Z axis) in the time domain.
* bodyAccelerationMagnitudeMeanByTime: Value between -1 and 1. Mean magnitude of the body acceleration gathered from the accelerometer in the time domain.
* gravityAccelerationMagnitudeMeanByTime: Value between -1 and 1. Mean magnitude of the gravity acceleration gathered from the accelerometer in the time domain.
* bodyAccelerationJerkMagnitudeMeanByTime: Value between -1 and 1. Mean Jerk magnitude of the body acceleration gathered from the accelerometer in the time domain.
* bodyAngularVelocityMagnitudeMeanByTime: Value between -1 and 1. Mean magnitude of the body angular velocity gathered from the gyroscope in the time domain.
* bodyAngularVelocityJerkMagnitudeMeanByTime: Value between -1 and 1. Mean Jerk magnitude of the body angular velocity gathered from the gyroscope in the time domain.
* bodyAccelerationMeanByFrequency_XAxis: Value between -1 and 1. Mean body acceleration gathered from the accelerometer (X axis) in the frequency domain.
* bodyAccelerationMeanByFrequency_YAxis: Value between -1 and 1. Mean body acceleration gathered from the accelerometer (Y axis) in the frequency domain.
* bodyAccelerationMeanByFrequency_ZAxis: Value between -1 and 1. Mean body acceleration gathered from the accelerometer (Z axis) in the frequency domain.
* bodyAccelerationJerkMeanByFrequency_XAxis: Value between -1 and 1. Mean Jerk body acceleration gathered from the accelerometer (X axis) in the frequency domain.
* bodyAccelerationJerkMeanByFrequency_YAxis: Value between -1 and 1. Mean Jerk body acceleration gathered from the accelerometer (Y axis) in the frequency domain.
* bodyAccelerationJerkMeanByFrequency_ZAxis: Value between -1 and 1. Mean Jerk body acceleration gathered from the accelerometer (Z axis) in the frequency domain.
* bodyAngularVelocityMeanByFrequency_XAxis: Value between -1 and 1. Mean body angular velocity gathered from the gyroscope (X axis) in the frequency domain.
* bodyAngularVelocityMeanByFrequency_YAxis: Value between -1 and 1. Mean body angular velocity gathered from the gyroscope (Y axis) in the frequency domain.
* bodyAngularVelocityMeanByFrequency_ZAxis: Value between -1 and 1. Mean body angular velocity gathered from the gyroscope (Z axis) in the frequency domain.
* bodyAccelerationMagnitudeMeanByFrequency: Value between -1 and 1. Mean magnitude of the body acceleration gathered from the accelerometer in the frequency domain.
* bodyAccelerationJerkMagnitudeMeanByFrequency: Value between -1 and 1. Mean Jerk magnitude of the body acceleration gathered from the accelerometer in the frequency domain.
* bodyAngularVelocityMagnitudeMeanByFrequency: Value between -1 and 1. Mean magnitude of the body angular velocity gathered from the gyroscope in the frequency domain.
* bodyAngularVelocityJerkMagnitudeMeanByFrequency: Value between -1 and 1. Mean Jerk magnitude of the body angular velocity gathered from the gyroscope in the frequency domain.
* bodyAccelerationStandardDeviationByTime_XAxis: Value between -1 and 1. Standard deviation of the body acceleration gathered from the accelerometer (X axis) in the time domain.
* bodyAccelerationStandardDeviationByTime_YAxis: Value between -1 and 1. Standard deviation of the body acceleration gathered from the accelerometer (Y axis) in the time domain.
* bodyAccelerationStandardDeviationByTime_ZAxis: Value between -1 and 1. Standard deviation of the body acceleration gathered from the accelerometer (Z axis) in the time domain.
* gravityAccelerationStandardDeviationByTime_XAxis: Value between -1 and 1. Standard deviation of the gravity acceleration gathered from the accelerometer (X axis) in the time domain.
* gravityAccelerationStandardDeviationByTime_YAxis: Value between -1 and 1. Standard deviation of the gravity acceleration gathered from the accelerometer (Y axis) in the time domain.
* gravityAccelerationStandardDeviationByTime_ZAxis: Value between -1 and 1. Standard deviation of the gravity acceleration gathered from the accelerometer (Z axis) in the time domain.
* bodyAccelerationJerkStandardDeviationByTime_XAxis: Value between -1 and 1. Standard deviation of the Jerk body acceleration gathered from the accelerometer (X axis) in the time domain.
* bodyAccelerationJerkStandardDeviationByTime_YAxis: Value between -1 and 1. Standard deviation of the Jerk body acceleration gathered from the accelerometer (Y axis) in the time domain.
* bodyAccelerationJerkStandardDeviationByTime_ZAxis: Value between -1 and 1. Standard deviation of the Jerk body acceleration gathered from the accelerometer (Z axis) in the time domain.
* bodyAngularVelocityStandardDeviationByTime_XAxis: Value between -1 and 1. Standard deviation of the body angular velocity gathered from the gyroscope (X axis) in the time domain.
* bodyAngularVelocityStandardDeviationByTime_YAxis: Value between -1 and 1. Standard deviation of the body angular velocity gathered from the gyroscope (Y axis) in the time domain.
* bodyAngularVelocityStandardDeviationByTime_ZAxis: Value between -1 and 1. Standard deviation of the body angular velocity gathered from the gyroscope (Z axis) in the time domain.
* bodyAngularVelocityJerkStandardDeviationByTime_XAxis: Value between -1 and 1. Standard deviation of the Jerk body angular velocity gathered from the gyroscope (X axis) in the time domain.
* bodyAngularVelocityJerkStandardDeviationByTime_YAxis: Value between -1 and 1. Standard deviation of the Jerk body angular velocity gathered from the gyroscope (Y axis) in the time domain.
* bodyAngularVelocityJerkStandardDeviationByTime_ZAxis: Value between -1 and 1. Standard deviation of the Jerk body angular velocity gathered from the gyroscope (Z axis) in the time domain.
* bodyAccelerationMagnitudeStandardDeviationByTime: Value between -1 and 1. Standard deviation magnitude of the body acceleration gathered from the accelerometer in the time domain.
* gravityAccelerationMagnitudeStandardDeviationByTime: Value between -1 and 1. Standard deviation magnitude of the gravity acceleration gathered from the accelerometer in the time domain.
* bodyAccelerationJerkMagnitudeStandardDeviationByTime: Value between -1 and 1. Standard deviation of the Jerk magnitude of the body acceleration gathered from the accelerometer in the time domain.
* bodyAngularVelocityMagnitudeStandardDeviationByTime: Value between -1 and 1. Standard deviation magnitude of the body angular velocity gathered from the gyroscope in the time domain.
* bodyAngularVelocityJerkMagnitudeStandardDeviationByTime: Value between -1 and 1. Standard deviation of the Jerk magnitude of the body angular velocity gathered from the gyroscope in the time domain.
* bodyAccelerationStandardDeviationByFrequency_XAxis: Value between -1 and 1. Standard deviation of the body acceleration gathered from the accelerometer (X axis) in the frequency domain.
* bodyAccelerationStandardDeviationByFrequency_YAxis: Value between -1 and 1. Standard deviation of the body acceleration gathered from the accelerometer (Y axis) in the frequency domain.
* bodyAccelerationStandardDeviationByFrequency_ZAxis: Value between -1 and 1. Standard deviation of the body acceleration gathered from the accelerometer (Z axis) in the frequency domain.
* bodyAccelerationJerkStandardDeviationByFrequency_XAxis: Value between -1 and 1. Standard deviation of the Jerk body acceleration gathered from the accelerometer (X axis) in the frequency domain.
* bodyAccelerationJerkStandardDeviationByFrequency_YAxis: Value between -1 and 1. Standard deviation of the Jerk body acceleration gathered from the accelerometer (Y axis) in the frequency domain.
* bodyAccelerationJerkStandardDeviationByFrequency_ZAxis: Value between -1 and 1. Standard deviation of the Jerk body acceleration gathered from the accelerometer (Z axis) in the frequency domain.
* bodyAngularVelocityStandardDeviationByFrequency_XAxis: Value between -1 and 1. Standard deviation of the body angular velocity gathered from the gyroscope (X axis) in the frequency domain.
* bodyAngularVelocityStandardDeviationByFrequency_YAxis: Value between -1 and 1. Standard deviation of the body angular velocity gathered from the gyroscope (Y axis) in the frequency domain.
* bodyAngularVelocityStandardDeviationByFrequency_ZAxis: Value between -1 and 1. Standard deviation of the body angular velocity gathered from the gyroscope (Z axis) in the frequency domain.
* bodyAccelerationMagnitudeStandardDeviationByFrequency: Value between -1 and 1. Standard deviation magnitude of the body acceleration gathered from the accelerometer in the frequency domain.
* bodyAccelerationJerkMagnitudeStandardDeviationByFrequency: Value between -1 and 1. Standard deviation of the Jerk magnitude of the body acceleration gathered from the accelerometer in the frequency domain.
* bodyAngularVelocityMagnitudeStandardDeviationByFrequency: Value between -1 and 1. Standard deviation magnitude of the body angular velocity gathered from the gyroscope in the frequency domain.
* bodyAngularVelocityJerkMagnitudeStandardDeviationByFrequency: Value between -1 and 1. Standard deviation of the Jerk magnitude of the body angular velocity gathered from the gyroscope in the frequency domain.

### Summary tidy data

The summary, uploaded to the coursera's project course page, is a computation of the average of each measurement values grouped by the variables ID_subject and activity.
It includes all the variables of the tidy data, except for the columns ID_activity (because it's not needed having the activity description already on the output) and  measurement_type (because it's not relevant to the summary required).