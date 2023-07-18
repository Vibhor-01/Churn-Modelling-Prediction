# Churn-Modelling-Prediction
This is a churn modelling project which uses Deep learning

In this Deep Learning project I have used a Deep Learning model to predict whether a customer will leave the bank or not. The model is trained on the dataset provided in this repository, and the model dataframe on which the model is trained uses a customer's creditScore, Geography, Gender, Age, Tenure, Balance, Number of products they own, Is and Active Member or not and Estimated Salary. The Traning Dataset does not include whether the customer has exited the company or not. That is allocated in a different variable ('y' in this case).

The Features of the Dataset are Encoded using LabelEncoder, OneHotEncoder, and ColumnTransformer. The ColumnTransformer is used in the Gender Column prominently, as it helpts to create 3 columns for genders and enter 1 wherever it is applicable.

The data is then Split into Train and Test in variations of 80% and 20%, with 80% being the Training set and 20% being the Test set. The split dataset are then scaled using Standard scaler.

The Deep Learning model is made using ANNs, containing 6 units and 1 unit of neuron each, and 'relu' as the activation function. The model contains 3 layers (more layers can be added if desired) with the first 2 layers containing 6 units of neurons, and the last layer consisting of 1 layer, as it is the output layer, and the output of this layer is either 1 or 0. The last layer uses 'sigmoid' activation funciton.

Lastly the model is compiled using 'adam' optimizer to perform stochastic gradient descent, 'binary_crossentropy' for loss estimation, and is trained with batch_size of 32 and epochs 100.

The model after training has an accuracy of 86.05% which can be increased depending on the programmer.
