# MedicalPrediction2025

## Problem Statement:
Missed appointments costs healthcare systems millions yearly. This project identifies key behavioral and demographic patterns behind patient no-shows using real clinical data.

## Objectives:
Cleaning and structuring raw clinical data from appointment dashboard
Performing EDA in finding operational issues
Performing Logistic Regression, Random Forest, and XGBoost in prediction analysis
Coming up with recommendations in lowering the No-Show rates

## Key Results:
* The XGBoost was the best model with a threshold of 0.488, compared to the Logistic Regression model (threshold of 0.46) and the Random Forest model(threshold of 0.49). The recall for patients who were labelled as 'no shows'(Class 1) was 0.78. This means out of all the no-shows the model correctly labelled those as no-show 78% of the time. The Logistic Regression model correactly labelled patients who were a no-show 68% of the time, and the Random Forest model it ws 24% of the time. This ultimately meant the XGBoost model was the best out of the three models. 
* The features that were most important in the XGBoost model (from most important to least) were:
  * Days Between (Days_Btwn)
  * Age
  * Texts Received (SMS_Received)
  * Poor/Working neighbourhood class (Neighbourhood_Class_Poor)
* The features that were most important in the Logistic Regression model (from most important to least) were:
  * Appointments on Saturdays (AppoinmentDOW_Saturday)
  * Appointment scheduled on Saturdays (ScheduledDOW_Saturday)
  * Days Between 
  * Days in Advance (Days_in_Advanced)
* The features that were most important in the Random Forest model (from most important to least) were:
  * Age
  * Days in Advance 
  * Days Between
  * SMS Recieved
