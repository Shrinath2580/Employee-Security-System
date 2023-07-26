# Employee-Security-System

Problem Statement:
You, as the Security analyst, at Stark Industries, have been tasked to build a new contactless 
employee check-in system. Currently the employees use a physical keycard for entry into 
the building like shown below.

You have come up with a new idea that uses the employees smartphone and machine learning to provide a contactless system where when an employee enters the firm’s territory, his or her smartphone connects to the server and transmits data from the employee smartphone sensor data like the accelerometer's data. The server performs the calculations and determines this person as one of the employees using Gait analysis. Essentially it compares the current pattern of the employee’s gait with the historical pattern and if there is a match, the doors automatically open for the employee to walk in.
To test your idea, you have built a dataset of 30 employees and their daily activities here. 
Design and develop a system that will perform the gait analysis.


Data Set Information:
The experiments have been carried out with a group of 30 volunteers within an age bracket of 19-48 years. Each person performed six activities (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING) wearing a smartphone (Samsung Galaxy S II) on the waist. Using its embedded accelerometer and gyroscope, we captured 3-axial linear acceleration and 3-axial angular velocity at a constant rate of 50Hz. The experiments have been video-recorded to label the data manually. The obtained dataset has been randomly partitioned into two sets, where 70% of the volunteers was selected for generating the training data and 30% the test data.
The sensor signals (accelerometer and gyroscope) were pre-processed by applying noise filters and then sampled in fixed width sliding windows of 2.56 sec and 50% overlap (128 readings/window). The sensor acceleration signal, which has gravitational and body motion components, was separated using a Butterworth low-pass filter into body acceleration and gravity. The gravitational force is assumed to have only low frequency components, therefore a filter with 0.3 Hz cut-off frequency was used. From each window, a vector of features was obtained by calculating variables from the time and frequency domain.
Check the README.txt file for further details about this dataset.
A video of the experiment including an example of the 6 recorded activities with one of the participants can be seen in the following link: [Web Link]
An updated version of this dataset can be found at [Web Link]. It includes labels of postural transitions between activities and the full raw inertial signals instead of the ones pre-processed into windows.


Attribute Information:
For each record in the dataset, it is provided:
- Triaxial acceleration from the accelerometer (total acceleration) and the estimated body acceleration.
- Triaxial Angular velocity from the gyroscope.
- A 561-feature vector with time and frequency domain variables.
- Its activity label.
- An identifier of the subject who carried out the experiment.


Proposed Work and Methodology:
The main idea behind this project is to create a seamless security system which is fast and 
yet is reliable with great precision. So, the main aspect that needs to be taken care of is the 
reliability and the accuracy of the system.

On doing an experiment on 30 employees, we have gathered their axis of their different 
body parts while they were doing their casual daily activities through the Gyroscope and 
Accelerometer that are present in their smartphones. Here the coordinates will be varying 
from every other individual as everyone has a different style of standing, walking, sitting, 
laying. Also, the body measurements of everyone are also different so by considering an 
individual’s body axis on how they enter the offices can help us to build a security system 
that is fast and secure.

While receiving all the required data through the individual's smartphone, we will now first analyse the data and then set the required parameters for training and prediction on different models for the same.

The main machine learning models that I have performed in this experiment are
1. LSTM
2. CNN-LSTM

After gathering what all features are given, we will train the model with 70% of the data as
training data and rest 30% of the data for prediction on the trained model.

The trained model then gave a model score of how it performed on the training dataset.

We run the model on the testing data and got a prediction score. A classification report for
the model was depicted. The analysis was summed up by a confusion matrix to evaluate the 
final performance of the algorithm.
