# Object Image Classification
######################################################################

This project automatically identifies the class of each image. 

20 objects classes with 5-20 examples each in different angles are used as training examples to train a CNN model with the following architecture

######################################################################

**Model Architecture**

Layer 1 : Conv2d Layer  (Kernel : (3x3))  (Stride : (1x1))  (Channels : 3->64)
Layer 2 : BatchNorm Layer                                   (Channels :64->64)
Layer 3 : ReLU Activation Output Layer                                        

Layer 5 : MaxPool Layer (Kernel : (2x2))  (Stride : (2x2))  (Channels :64->64)

Layer 5 : Conv2d Layer  (Kernel : (3x3))  (Stride : (1x1))  (Channels :64->64)
Layer 6 : BatchNorm Layer                                   (Channels :64->64)
Layer 7 : ReLU Activation Output Layer                                       

Layer 8 : MaxPool Layer (Kernel : (2x2))  (Stride : (2x2))  (Channels :64->64)

Layer 9 : Conv2d Layer  (Kernel : (3x3))  (Stride : (1x1))  (Channels :64->128)
Layer 10 :BatchNorm Layer                                   (Channels :128->128)
Layer 11 :ReLU Activation Output Layer                                       

Layer 12 :MaxPool Layer (Kernel : (2x2))  (Stride : (2x2))  (Channels :128->128)

Layer 13 :Conv2d Layer  (Kernel : (3x3))  (Stride : (1x1))  (Channels :128->128)
Layer 14 :BatchNorm Layer                                   (Channels :128->128)
Layer 15 :ReLU Activation Output Layer                                        

Layer 16 :MaxPool Layer (Kernel : (2x2))  (Stride : (2x2))  (Channels :128->128)

Layer 17 :Conv2d Layer  (Kernel : (3x3))  (Stride : (1x1))  (Channels :128->20)
Layer 18 :BatchNorm Layer                                   (Channels : 20->20)
Layer 19 :ReLU Activation Output Layer    

######################################################################

######################################################################

**Model Optimization** 

Loss : Cross Entropy
Optimizer : SGD (lr : 0.001, momentum : 0.9)

######################################################################

######################################################################

**Results**

Avg loss (train): 0.0029
Avg acc (train): 0.9983
Avg loss (test): 0.0069
Avg acc (test): 0.9567



Training completed in 11m 43s
Best acc: 0.9567

######################################################################


