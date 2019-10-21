# Standardized Image data Classification using CNN
##############################################################################

Design a convolutional neural network for the dataset provided. It contains 60000 training (training_data.npy) and 10000 test (test_data.npy) examples. The training examples are labeled (training_label.npy) with 10 different classes. Training as well as testing data is in format: numpy list of flattened image pixel values. Length of axis 0 is 60000( training data) and length of axis 1 is 784(number of pixels of each image). 
#########################################

The Train Data is split into ----> Validation + Train (0.33:0.67) where Train is again split into Train + Val (0.2:0.8)

Both the Train and Test data are standardized

The Labels are "ONE HOT ENCODED"

#########################################

#########################################

##### Model architecture

Convolutional Layer (3x3)x16 RELU
Convolutional Layer (3x3)x16 RELU

MaxPool Layer (2x2)

Convolutional Layer (5x5)x32 RELU
Convolutional Layer (5x5)x32 RELU

MaxPool Layer (2x2)

Dropout Layer 0.3

Dense Layer 1024 RELU

Dense Layer 10 SOFTMAX

#########################################

#########################################

##### Model Optimization 

Loss : Categorical Crossentropy
Optimizer : ADAM
Metric : Categorical Accuracy

#########################################

#########################################

##### Model Observations 

Model starts to overfit after 8th epoch

Model Training Accuracy : 95.11%

Model Val Accuracy : 91.64%  <---- Split from X_train

Model Validation : 91.621% <---- Split from Test Data

##############################################################################








