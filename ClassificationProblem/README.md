# Arya.ai DS Assignment. 

The Notebook is divided into following sections. 
1. Import, Utility functions are designed here.
2. Data Load Part. 
   1. Data is loaded into raw_data_dict
      1. can be accessed using "test" and "train" keys.
3. Exploratory Data Analysis. 
   1. Checking for missing data - None Found
   2. Checking for outliers - There were quite a few columns having very skewed data.
   3. There were lots of columns having zero values. 
   4. It looked like the columns from X1-X54 was from one single source. after adding all could observe normal distribution.
   5. Analysing each of these columns with Target Variable using box plot. There was a relation between outlier values with either of the binary class. 
   6. Initial thought process was to apply one of dimensionality reduction techniques. 
4. Data Split.
   1. Train data was further split into two - Train and validation, with 80% data in train and rest in validation
   2. The target's value counts in validation set was almost same as the one in train set.
5. Modeling 
   1. To use all features.
   2. Auc score is used to evaluate the models. 
   3. out of all different ml techniques, RFC and XGB was performing better than others. 
hence decided to go ahead with these to techniques for model tuning.
6. Model Tuning.
   1. Tuned model - RFC was giving 94% accuracy on validation data set.
   2. Tuned model - XGB was giving 96% accuracy on validation data set. 

Other data with creating column, if that column contains a zero or some other number. here the perf was almost close to the previous one.

Test set prediction is done using Tuned XGB model. 

All the packages required are placed in req.txt file. 


        