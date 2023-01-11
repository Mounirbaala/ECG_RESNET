# ECG_RESNET
This is a code defines a convolutional neural network (CNN) using the Keras library in Python. 
The network begins with an input layer that has a shape of (1, 570, 33), 
meaning it expects to receive an input of 1 image, with 570 pixels in the x-dimension, and 33 pixels in the y-dimension.
The model then applies a series of convolutional, batch normalization, activation, and dropout layers in a pattern that is repeated three times, 
with each repetition resulting in a new output block. The number of feature maps, which represent the number of filters in the convolutional layers,
starts at 64 and doubles with each repetition. The kernel size, which is the size of the window that slides over the input image, 
also changes throughout the layers, with values of 8, 5, and 3. Additionally, the activation function for each repetition is ReLU, 
and dropout rate is 0.3. The output of each block is calculated by adding the output of the convolutional layers with the output from the shortcut.

