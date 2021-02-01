# GEEMAP
Machine Learning with Earth Engine - Supervised Classification
Supervised classification algorithms available in Earth Engine
Source: https://developers.google.com/earth-engine/classification

The Classifier package handles supervised classification by traditional ML algorithms running in Earth Engine. These classifiers include CART, RandomForest, NaiveBayes and SVM. The general workflow for classification is:

Collect training data. Assemble features which have a property that stores the known class label and properties storing numeric values for the predictors.
Instantiate a classifier. Set its parameters if necessary.
Train the classifier using the training data.
Classify an image or feature collection.
Estimate classification error with independent validation data.
The training data is a FeatureCollection with a property storing the class label and properties storing predictor variables. Class labels should be consecutive, integers starting from 0. If necessary, use remap() to convert class values to consecutive integers. The predictors should be numeric.
