# Tensorflow
Using tensorflow CNN to Predict IDC in Breast Cancer Histology Images
Dataset : Breast Histology Images  (Classify IDC vs non IDC images)
https://www.kaggle.com/simjeg/lymphoma-subtype-classification-fl-vs-cll
CNN Model (Lenet)
Input layer: [., 50, 50, 3]
layer: Conv1 -> ReLu -> MaxPool: [., 25, 25, 36]
layer: Conv2 -> ReLu -> MaxPool: [., 13, 13, 36]
layer: Conv3 -> ReLu -> MaxPool: [., 7, 7, 36]
layer: FC -> ReLu: [., 576]
output layer: FC -> ReLu: [., 2]
Multilayer Perceptron
Input layer: (., 50, 50, 3)
hidden layer 1 = 512,
hidden layer 2 = 256,
hidden layer 3 = 128,
Output: 2
We compare two results of different neural network architectures.
The neural network is implemented as a python class and the complete TensorFlow session can be saved to or restored from a file.
We also implement tensor summaries, which can be visualized with TensorBoard. 
The output layer gives for each image a probability for IDC=0 and IDC=1. 
