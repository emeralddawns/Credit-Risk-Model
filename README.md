# supervised-machine-learning
This assignment consisted of python, pandas, and sklearn to build a machine learning model.

# What the code does (in general terms)
The code pre-processes the data by turning categorical data to numeric columns, creating a dummy column where needed, fitting the data to  LogisticRegression model and a RandomForestClassifier model, and printing out the score. Then the data is further processed by scaling the numeric columns, fitting the models again, and printing out the score.  Predictions were made before each step and used for analysis

# Analysis

Regarding the testing score, the methods performed as follows:

    Logistic Regression, Scaling Testing Data Score: 0.7201190982560612

    Random Forest, Scaling Testing Score: 0.6193109315185028

    Random Forest, No Scaling Testing Score: 0.6180348787749894

    Logistic Regression, No Scaling Testing Data Score: 0.5253083794130158

Prediction 1: Logistic Regression will perform better than Random Forests before scaling because the data has more continuous variables than categorical variables - ### Incorrect

Prediction 2: Scaling will improve the model score as it should reduce the tendency of the models to 'bias' torwards higher numbers - ### No change for Random Forests (difference of 0.001), Correct for Logistic Regression

Prediction 3: Logistic Regression will perform better than Random Forests after scaling because scaling helps Logistic Regression more than Random Forests - ### Correct

Learning: Not all models have a bias towards higher value numbers. Logistic Regression does and should, therefore, use scaled features. Random Forests Classification does not have this bias, however.
