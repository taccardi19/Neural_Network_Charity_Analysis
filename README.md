# Neural_Network_Charity_Analysis

## Project Overview
The purpose of this project is to use neural networks with the TensorFlow platform in Python to analyze and classify the success of charitable donations.
We use the following methods for the analysis:

- Preprocessing the data for the neural network model
- Compile, train and evaluate the model
- Optimize the model

## Results

### Data Preprocessing
- To begin, columns EIN and NAME are identification information and have been removed from the input data.
- The column IS_SUCCESSFUL contains binary data refering to whether or not the charity donation was used effectively so this variable is considered as the target for our deep learning neural network.
- The following columns APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT are the features for our model.
- Encoding of the categorical variables, spliting into training and testing datasets and standardization have been applied to the features.

### Compiling, Training, and Evaluating the Model
- This deep-learning neural network model is made of two hidden layers with 80 and 30 neurons respectively.
- The input data has 43 features and 25,724 samples.
- The output layer is made of a unique neuron as it is a binary classification.
- To speed up the training process, we are using the activation function ReLU for the hidden layers. As our output is a binary classification, Sigmoid is used on the output layer.
- For the compilation, the optimizer is adam and the loss function is binary_crossentropy.
- The model accuracy is under 75%. This is not a satisfacory output to help predict the outcome of the charity donations.
- To increase the performance of the model, we added back the "NAME" field into our dataset.
- After this optimization, we got a 97% model accuracy, which is a satisfactory output to predict the outcome of the charity donations.


## Summary
The deep learning neural network model did not reach the target of 75% accuracy initially. After our optimization method, however, we got a 97% accuracy and are satisifed with this deep learning model. Another way we could improve classifications is by using a supervised machine learning model such as the Random Forest Classifier to combine a multitude of decision trees to generate a classified output and evaluate its performance against our deep learning model.
