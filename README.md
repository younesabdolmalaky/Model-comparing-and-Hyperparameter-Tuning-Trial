# Model-comparing-and-Hyperparameter-Tuning-Trial
# About the dataset
The data points were collected from a Combined Cycle Power Plant over 6 years (2006-2011) when the power plant was set to work with a full load. Features consist of hourly average ambient variables - Ambient Temperature (AT), Ambient Pressure (AP), Relative Humidity (RH) and Exhaust Vacuum (V) to predict the net hourly electrical energy output (PE) of the plant.

A combined-cycle power plant uses both gas and a steam turbine together to produce up to 50 percent more electricity from the same fuel than a traditional simple-cycle plant. The waste heat from the gas turbine is routed to the nearby steam turbine, which generates extra power.

All the UN Member States have to submit a report on the combined cycle power plant to the United Nations. The Power Plant officials of Mexico are devising a way to predict the net hourly electrical energy output (PE) of the plant. You are appointed as the chief for this operation. Create a Machine Learning Model to solve this problem efficiently.

#Introduction¶

Single-cycle gas turbine power plants generate electricity by using natural gas and compressed air. Air is drawn from the surroundings, compress ed, and fed into the combustion chamber of the gas turbine. Here, natural gas is injected which mixes with the compressed air and ignited. The combustion produces a high-pressure, hot gas stream that flows through the turbine causing it to spin (at tremendous speeds). Consequently, this spins a generator which is connected to the turbine to produce electricity. For single-cycle gas turbines, much of the energy is wasted as hot exhaust achieving an energy conversion efficiency of 35% at best. Combined cycle power plants exploit this inefficiency by capturing the waste heat using a heat recovery steam generator (HRSG), to produce even more power. Combined cycle power plants are power generation plants that use both gas and steam turbines together to generate electricity. The waste heat generated from the gas turbine is used to produce steam which is fed to a steam turbine to generate even more electricity. This increases the power produced (up to 50% more) for the same amount of fuel, as well as increases the plant’s efficiency to about 60%. The Output power of the Combined Cycle Power Plant (CCPP) is dependent on a few parameters which are atmospheric pressure, exhaust steam pressure, ambient temperature, and relative humidity. Being able to predict the full load electrical power output is important for the efficient and economic operation of the power plant.

![download](https://user-images.githubusercontent.com/75095471/217403841-9d5596d8-0224-4a76-bbe3-97788a9600cd.png)

# Algorithms Overview
## Linear Regression:
Linear regression is a simple and classic regression algorithm. It tries to fit a line to the data that minimizes the sum of the squared differences between the true values and the predicted values. The mathematical formula for linear regression can be represented as y = b0 + b1x1 + b2x2 + ... + bn*xn, where b0, b1, b2, ..., bn are the coefficients and x1, x2, ..., xn are the independent variables.

## Decision Tree:
Decision tree is a simple and easy to interpret tree-based algorithm. It recursively splits the data into subsets based on the feature that provides the highest reduction in impurity. The mathematical formula for decision trees is based on entropy and information gain.

## Random Forest:
Random forest is an ensemble algorithm that uses multiple decision trees to make a prediction. The prediction is made by aggregating the predictions of each individual tree, typically by taking the average. Random forest improves upon decision trees by reducing overfitting and improving generalization.

# K-Nearest Neighbors:
 K-Nearest Neighbors is a simple and intuitive non-parametric algorithm. It predicts the target variable for a new sample based on the average of the k nearest samples in the training set. The mathematical formula for KNN is based on the Euclidean distance between samples.

# Support Vector Regression:
 Support Vector Regression is a variation of Support Vector Machines that is used for regression. It tries to fit a hyperplane that maximizes the margin between the samples and the hyperplane. The mathematical formula for SVR is based on the optimization of a convex cost function.

# CatBoost: 
CatBoost is a gradient boosting algorithm specifically designed for categorical data. It uses a combination of decision trees and gradient descent to make predictions. The mathematical formula for CatBoost is based on gradient boosting and decision trees.

# XGBoost: 
XGBoost is another gradient boosting algorithm that is widely used in data science. Like CatBoost, it also uses gradient boosting with decision trees as its base model.
# Deep Learning Neural Network:
Deep Learning Neural Network (DLNN) is a type of artificial neural network (ANN) that is designed to mimic the structure and function of the human brain. It consists of multiple interconnected processing nodes, or neurons, that are organized into layers. The input layer receives the input data, and the output layer produces the prediction. The hidden layers are responsible for transforming the input into a form that can be used by the output layer to make the prediction. The neurons in each layer are connected to the neurons in the next layer through weighted connections, and the weights are adjusted during training to minimize the difference between the true and predicted values. DLNNs are capable of learning complex relationships in the data and can be used for a variety of tasks, including classification and regression. The mathematical formula for DLNNs involves the computation of dot products, activation functions, and backpropagation of errors for weight adjustment.
