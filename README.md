# Cats and Dogs Classification using Convolutional Neural Networks

![Cats   dogs](https://github.com/Emilija453/cat_dog_cnn/assets/123960017/1546f2c9-92e8-475a-80f9-376e3190a833)

## Overview!


This project demonstrates a Convolutional Neural Network (CNN) model built with TensorFlow and Keras to classify images of cats and dogs. The model is trained on a dataset containing 2000 images for training, 1000 images for validation, and 50 images for testing.

## Data Preprocessing

Images are preprocessed using `ImageDataGenerator` to perform the following operations:
- Rescale the image pixel values to the range [0, 1].
- Augment the training data with random rotations, shifts, shears, zooms, and horizontal flips.

## Model Architecture

The CNN model architecture consists of the following layers:
1. **Conv2D** with 32 filters, relu activation
2. **MaxPooling2D**
3. **Conv2D** with 64 filters, relu activation
4. **MaxPooling2D**
5. **Conv2D** with 128 filters, relu activation
6. **MaxPooling2D**
7. **Flatten**
8. **Dense** with 512 units, relu activation
9. **Dense** with 1 unit, sigmoid activation

The model is compiled with:
- **Optimizer**: Adam
- **Loss function**: Binary Crossentropy
- **Metrics**: Accuracy

## Training

The model is trained for 15 epochs with a batch size of 128. Training history shows the progression of training and validation accuracy and loss over epochs.

## Evaluation

The model's performance is evaluated on the test set, and the results show that the model correctly identified 74.0% of the images of cats and dogs.
