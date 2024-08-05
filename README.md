# Concrete Strength Prediction with Regression and Neural Networks

## Project Overview
This GitHub project showcases the development, training, and evaluation of regression models to predict the strength of concrete based on various ingredients and age. The dataset includes features such as Cement, Blast Furnace Slag, Fly Ash, Water, Superplasticizer, Coarse Aggregate, Fine Aggregate, Age, and Strength. Four parts of the project are outlined below:

### Part A
In Part A, we create, train, and evaluate a regression model using the raw dataset without any normalization or scaling of predictor variables. This code allows us to see the initial model performance with unaltered feature values.

### Part B
Part B focuses on data preprocessing. The predictor variables are normalized by subtracting the mean and dividing by the standard deviation for each feature. This normalization ensures that all features have a mean of zero and a standard deviation of one, bringing them to the same scale for training.

### Part C
Part C explores the impact of training duration. It extends the training period to 100 epochs, providing the model with more opportunities to learn from the data. Additionally, this code repeats the training and evaluation process 50 times, calculating the mean and standard deviation of the mean squared errors. This approach provides a more robust estimate of model performance.

### Part D
Part D presents a comprehensive process using the Keras library to build, train, and evaluate a neural network model. The dataset is loaded, explored, and preprocessed. Predictors (features) are normalized to have zero mean and unit variance. The model consists of three hidden layers, each with 10 nodes and ReLU activation functions. The model is compiled with the Adam optimizer and mean squared error as the loss function. Training occurs over 50 epochs, and performance is evaluated using mean squared error. The entire process is repeated 50 times, calculating the mean and standard deviation of mean squared errors.

### Final Keras Assignment
This part represents the entire series of experiments designed to understand the impact of different factors on the performance of a neural network model for a regression problem, with the regression problem at hand being predicting the strength of concrete based on certain predictors.

Each part explores a different aspect of model development and evaluation:

1. Building a baseline model: This part creates a simple neural network model with one hidden layer of 10 nodes and a ReLU activation function. The model is trained on a randomly split dataset and evaluated on a test set. The mean squared error (MSE) between the predicted and actual concrete strengths is computed and reported. This process is repeated 50 times to create a list of MSEs, which are then used to compute and report the mean and standard deviation of the MSEs.
2. Normalizing the data: The predictors are normalized by subtracting the mean and dividing by the standard deviation. This process is repeated for the model training and evaluation as in the first part, but with the normalized data. The MSEs are computed in the same way and compared to those from the first part.
3. Increasing the number of epochs: The number of training epochs is increased from 50 to 100. The MSEs are computed in the same way as in the previous parts and compared to those from the second part.
4. Increasing the number of hidden layers: The model is modified to include three hidden layers, each with 10 nodes. The MSEs are computed in the same way as in the previous parts and compared to those from the third part.

The purpose of these experiments is to understand how different aspects of model development and evaluation, such as data normalization, the number of training epochs, and the architecture of the neural network, can impact the performance of the model in predicting concrete strength. The results from these experiments provide insights into the best practices for developing and evaluating neural network models for regression problems.

## How to Use
To explore this project and its code, follow these steps:

1. Clone the repository to your local machine.
2. Navigate to the desired part (A, B, C, or D) in the project directory.
3. Execute the provided code files to run the specific experiment.
4. Examine the code and results to gain insights into regression modeling and neural networks.
5. Experiment with changing the method parameters (e.g., number of epochs, number of hidden layers, normalization) to observe how these variations impact the results, including mean and standard deviation of mean squared errors and other relevant metrics.

## License
This project is open-source and available under the MIT License. Review the license for detailed terms and conditions.
