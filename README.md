# csci-585
#HW3:Geospatial data handling

Collect latitude,longitude pairs (ie. spatial coordinates) for 15 locations, in the USC campus (UPC). Sample 5 points, in 3 categories of your choice - libraries, cafes, waterworks, etc. 
Create KML file with these 15 locations and  use Google Earth to visualize the data in your KML file.
Use spatial db software-PostGres to compute the convex hull for the 15 points [a convex hull for a set of 2D points is the smallest convex polygon that contains the point set].
Compute the four nearest neighbors of one of the 15 locations 
Use OpenLayers (a JavaScript API) to visualize your location data.
Using one of the location as centre , compute a set (sequence) of lat-long (ie. spatial) co-ordinates that lie along a Spirograph(TM) curve 
Use ArcGIS' online map creator to view your Spirograph curve-shaped points

#HW4: Data Mining, tool-based
a) Weka
Dataset used:'Boston Housing Dataset' 
This dataset that contains data regarding houses in several Boston suburbs, published in 1993. It has 506 rows (records) of data, and 14 columns (attributes).
Predict: 'MEDV' (median home price) 
1. Build a linear regression equation, to predict MEDV. 
2. Create a 'MultilayerPerceptron' neural network that learns the data and find Root Mean Squared Error
b) KNIME:
Dataused :Abalon shells.
It consists of 4177 rows of data regarding abalone shells, where each row resulted from measuring 9 parameters/features/values for each shell. The data is in text format (.arff format). The idea is to be able to predict the 9th value, number-of-rings, given the other 8 values, using the existing dataset to learn how to predict.
1.Perform linear regression [on all parameters, not a subset] using nodes: AARF Reader, Linear Regression Learner. Create and connect the nodes, and execute each. Generate its linear regression equation
2.Set up a 'Decision Tree Learner' predictor, where 'sex' is the predicted variable. 
c)Rapid Miner:
1. Create 6 clusters  out of the 4177 pieces of data (use a kMeans 'Clustering' node). Find data points in each cluster
2. Find linear regression to predict num_rings, from length,diameter,height.

#HW 5 :Supervised machine learning
Train a neural network on differentiating between a cat pic and dog pic, then use the trained network to classify a new (cat-like or dog-like) pic into a cat or dog. 
The code uses the Keras NN library, which runs on graph (dataflow) execution backends such TensorFlow(TF), Theano, CNTK [here i am running it over TF via the Google cloud


