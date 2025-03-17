CIFAR-10 Image Classification with CNN

This project implements a Convolutional Neural Network (CNN) using TensorFlow and Keras to classify images from the CIFAR-10 dataset.

Requirements

Ensure you have the following dependencies installed:

pip install tensorflow matplotlib

Dataset

The CIFAR-10 dataset consists of 60,000 32x32 color images in 10 classes, with 6,000 images per class. It is automatically downloaded using TensorFlow.

Model Architecture

The CNN consists of:

Three convolutional layers with ReLU activation

Two max-pooling layers

A fully connected dense layer

A final output layer with 10 classes


Training

The model is trained using:

Adam optimizer

Sparse categorical crossentropy loss

Accuracy as the evaluation metric


history = model.fit(train_images, train_labels, epochs=10,
                    validation_data=(test_images, test_labels))

Evaluation

After training, the model is evaluated on the test set:

test_loss, test_acc = model.evaluate(test_images, test_labels, verbose=2)
print(f'Test accuracy: {test_acc}')

Results

The model achieves around 71.5% accuracy on the CIFAR-10 test dataset after 10 epochs.
