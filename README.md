# Image-Classification-

Overview
In this project, I leveraged TensorFlow's Keras API to create a sequential model that processes, normalizes, and classifies images of cats and dogs with impressive accuracy.

Requirements
To run this project, I needed a few key libraries:

TensorFlow for building and training neural networks.

Keras as part of TensorFlow for model creation.

Matplotlib for visualizing training results.

Pillow (PIL) for image processing.

These libraries can all be installed via pip, making setup straightforward.

Dataset
The dataset is composed of images of cats and dogs, which are split into training and validation sets. The images are organized into directories to facilitate easy loading and labeling by the Keras API.

Preprocessing
To prepare the images for training, they are divided into batches and normalized. This step ensures that the data is efficiently managed and that the pixel values are scaled to a range suitable for neural network processing.

Model Architecture
The heart of this project is the CNN model, which I constructed in a sequential manner. The model starts with convolutional layers that detect various patterns and features in the images. These are followed by max-pooling layers that reduce the size of the feature maps, making the model more efficient and less prone to overfitting.

After the convolutional and pooling layers, the model flattens the multidimensional data into a 1D array, ready for the dense (fully connected) layers. These dense layers further process the data, culminating in an output layer that uses a sigmoid activation function to classify the images into two categories: cats or dogs.

Compiling the Model
Before training, I compiled the model using the Adam optimizer, which adjusts the model's weights to minimize the loss function. The binary cross-entropy loss function is used since we are dealing with a binary classification task. The model's accuracy is tracked during training to monitor performance.

Training
The model was trained over a series of epochs, where it learned to classify the images by adjusting its weights based on the training data. The validation set was used to ensure the model generalizes well to new, unseen data.

Visualization
To understand how well the model is performing, I plotted the training and validation accuracy over the epochs. This helps in visualizing the model's learning progress and identifying any potential issues like overfitting.

