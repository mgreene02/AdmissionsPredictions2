# AdmissionsPredictions2
This goal of this project is to use pre-processing and ML pipelines to predict an indivudual's admissability to a particular university. 
The data is from prospective university applicants, who are given a subjective scored based on their academic profile. 

WARNING:
--------
The parameters of this dataset are greatly simplified and are in no way representative of actual admissions decisions procedures. This report is for educational purposes only, and is not meant to represent any procedure adopted by any university. 
--------


The dataset used is actual proprietaty data, but the project below uses public data with similar procedures: 
https://www.kaggle.com/mgreene02/predicting-university-admissions-decisions?scriptVersionId=6991775

There is one key difference, however. Instead of predicting binary admissions decisions there, here I am predicting on a scale of 1-5 an admissibility index. 

The metric used to evaluate predictive capabiltiy is accuracy, as well as a custom metric which I call plus or minus 1. since we are predicting a value between 1 and 5, I also would like to know how many predictions are within one value. 
This metric will be reported as (X, Y), where X is the exact accuracy (outcome == prediction), and Y is the plus or minus accuracy, (outcome == prediction, or outcome == prediction+1, or outcome == prediction-1)
