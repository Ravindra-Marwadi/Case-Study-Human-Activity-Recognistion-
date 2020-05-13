# HUMAN-ACTIVITY-RECOGNITION
This project is to build a model that predicts the human activities such as Walking, Walking_Upstairs, Walking_Downstairs, Sitting, Standing or Laying. This dataset is collected from 30 persons(referred as subjects in this dataset), performing different activities with a smartphone to their waists. The data is recorded with the help of sensors (accelerometer and Gyroscope) in that smartphone. This experiment was video recorded to label the data manually. got data from [here](https://archive.ics.uci.edu/ml/datasets/human+activity+recognition+using+smartphones)
### How data was recorded:  
Video Source: https://www.youtube.com/watch?v=XOEN9W05_4A&feature=youtu.be

By using the sensors(Gyroscope and accelerometer) in a smartphone, they have captured '3-axial linear acceleration'(tAcc-XYZ) from accelerometer and '3-axial angular velocity' (tGyro-XYZ) from Gyroscope with several variations. The sensor signals (accelerometer and gyroscope) were pre-processed by applying noise filters and then sampled in fixed-width sliding windows of 2.56 sec and 50% overlap (128 readings/window). The sensor acceleration signal, which has gravitational and body motion components, was separated using a Butterworth low-pass filter into body acceleration and gravity. The gravitational force is assumed to have only low frequency components, therefore a filter with 0.3 Hz cutoff frequency was used. From each window, a vector of features was obtained by calculating variables from the time and frequency domain.
### Attribute Information:  
For each record in the dataset it is provided: 
- Triaxial acceleration from the accelerometer (total acceleration) and the estimated body acceleration. 
- Triaxial Angular velocity from the gyroscope. 
- A 561-feature vector with time and frequency domain variables. 
- Its activity label.(WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING)
- An identifier of the subject who carried out the experiment.  

### Results:  
##### With Handcoded 561 Features and Machine Learning Algorithms
| Algorithm        | Test Accuracy % | 
| ------------- |-------------|
| Logistic Regression      | 96.3 |
| Linear SVC      | 96.5      | 
| rbf SVM classifier      | 96.27      | 
| DecisionTree      | 86.39      | 
| Random Forest      | 91.08      | 
| GradientBoosting DT      | 92.63      | 
##### With Raw Series data and Deep Learning model 
![image](https://user-images.githubusercontent.com/40149802/65963597-bbd4ba80-e478-11e9-88be-0c4e59b6d32a.png)


References:
1. Deep Learning Models for Human Activity Recognition by machinelearningmastery.com
2. Applied Ai Course
3. Divide and Conquer-Based 1D CNN Human Activity Recognition Using Test Data Sharpening [paper]( https://www.mdpi.com/1424-8220/18/4/1055/pdf )
