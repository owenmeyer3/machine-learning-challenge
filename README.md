# Overview - Exoplanet Exploration
This project analyzes exoplanet exploration data. The data set gives values for 20 features and a classification for the status of the planet ('False Positive', 'Candidate' or 'Confirmed). Multiple machine models will be used to evaluate the optimal model for this categorical solution.

## Models
1. All models first break the exoplanet exploration data into feature data and target data. The data is split into training data and testing data.
2. Preprocessing is preprocessed to scale feature data with a MinMaxScaler, in order to normalize data on a 0.0 to 0.1 scale. Target data is one-hot encoded, which is needed for target data with more than 2 categories.

### Logistic Regression
1. The Logistic Regression model is fit to the training data and evaluated for accuracy.
2. The same Logictic model is tuned with gradient descent to modify optimizer parameters. The model is then fit to training data.
3. Both the base logistic regression model and the gradient descent applied model are tested with test data and compared to see if there is considerable improvement with implementation of gradient descent

### Support Vector Machine (SVM)
The SVM model uses a strategy as the Logistic regression model. Instead of implementing a logistic regression model, the SVM model is used. Gradient descent is applied to the SVM model as well.

### Neural Net
The neural net uses as sequential model. In this project, inputs go through one hidden layer before reaching the output. A classification method is used to evaluate the accuracy of the model. Gradient descent is not an extra step for this model.

## Evaluation