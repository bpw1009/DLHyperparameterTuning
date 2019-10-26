# DLHyperparameterTuning
This notebook shows an approach to hyperparameter tuning for deep learning with Keras.

This assignment was to create synthetic data to train deep learning models using keras, and to systematically test different hyperparameter settings. 

There were two phases to this asignment.
1. Focus on Batch Size, Activation Functions, and Number of Nodes / Layers
2. Focus on Optimizers, Weight Initialization, and Dropout

# Requirements for each phase
## Phase 1
•	Batch Size  = [8, 16, 32]

•	Activation Functions = [Sigmoid, ReLU, Leaky ReLU]
model.add(LeakyReLU(alpha=.001))   # use case example

•	Number of Nodes / Layers = [10, 20, 50] / [1,2]
Don’t use weight initialization or Dropout for this phase. Use RMSProp optimizer throughout for this phase.  

## Phase 2
Choose fixed settings for the parameters from Phase 1 as follows:

•	Batch Size = 32

•	Activation functions for hidden layers = ReLU

•	Number of nodes / hidden layers = 50 / 1

The variable setting are as follows:

•	Optimizers = [SGD, RMSProp, ADAM] # use settings as recommended by the Keras documentation

•	Weight Initialization = [Xavier_uniform, Xavier_Normal, He_uniform, He_Normal]

•	Dropout = [0.2, 0.4, 0.5]


