# Detection-of-Panic-Attacks


This Classifier is a component of bigger project I worked on with a team in my third year. Files that can be found here contain code and results of:
- accelerometer and gyroscope data pre-processing (including downsampling and filtering).
  - downsampling was first preformed at rate of 50Hz.
  - then, we used moving-average window to reduce the rate to 3Hz.
  - performed low-pass, median, and combined (low-pass+median) filters on the data
  * Used Shimmer Sample Data for visualisation and simplified testing
- traditional activity classification method.
  - five machine learning models were tested (logistic regression, Kernel SVM, Decision tree, Random Forest Classifier, Linear SVC)
  - used grid search to find optimal hyperparameters
- data analysis for the purpose of optimizing classifier for the purpose.
  - plotted various dependencies in the data in order to find certain repetitivity and groups that could be used to improve classification for the specific purpose of our device
- optimized version of activity classifier that decides in which heart-rate-range group activity belongs to rather than classifying the activity itself.
