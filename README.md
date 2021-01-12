# Pulsar-Stars
I trained some Supervised learning models to predict a pulsar star and explained why i would use the models i did for this particular task.
The dataset I used for this research was developed by Pavan Raj and downloaded from Kaggle.

The data contains 12,510 datapoints with 1,153 positive targets and 11,357 false target observations
 this data has 9 columns that we will describe briefly here. The data contains the following columns:
 
Mean of the integrated profile.
Standard deviation of the integrated profile.
Excess kurtosis of the integrated profile.
Skewness of the integrated profile.
Mean of the DM-SNR curve.
Standard deviation of the DM-SNR curve.
Excess kurtosis of the DM-SNR curve.
 Skewness of the DM-SNR curve.
Class

The first four columns are measured attributes of the stars and the last four are obtained by some statistical calculations on the DM-SNR curve. The features are all continuous as well. Dispersion-measure-signal-to-noise-ratio(DM-SNR) is a calculated measure using the image of stars. The Integrated profile, also known as the integrated intensity profile, is a standard tool in image analysis. 

We will model this problem as a binary classification problem. I will use a variety of classifiers like KNN, Random Forest, Support Vector Machines, and Gradient Boosting to see how well we can get them to perform the task and then settle on the best performing one to put forward as a possible implementation for identifying pulsar stars. We will primarily use the sklearn classification report to compare models and specifically, the recall score. 
Some EDA had to be performed to clean the dataset before modeling and I d like to share some insights about the raw data before continuing to the modeling portion 
