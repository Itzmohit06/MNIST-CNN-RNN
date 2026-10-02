# Handwritten Digit Classification using CNN and RNN

This project focuses on recognizing handwritten digits from the MNIST dataset using two different deep learning approaches: a Convolutional Neural Network (CNN) and a Recurrent Neural Network (RNN).

The main goal of the project is to understand how CNN and RNN models work for image classification and compare their performance on the same dataset.

## About the Project

Handwritten digit recognition is a common image classification problem where the model needs to identify digits from 0 to 9.

In this project, I trained:

- A CNN model for extracting spatial features from handwritten digit images.
- An RNN model by treating the image rows as a sequence.
- An improved RNN model to check whether changes in the architecture and training setup could improve its performance.

The models were trained and tested using the MNIST dataset.

## Dataset

The project uses the **MNIST handwritten digit dataset**.

- Training images: 60,000
- Test images: 10,000
- Image size: 28 × 28 pixels
- Number of classes: 10 (digits 0–9)

The original training data was divided into training and validation sets:

- Training: 54,000 images
- Validation: 6,000 images
- Testing: 10,000 images

## Technologies Used

- Python
- PyTorch
- Torchvision
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Project Structure

```text
MNIST-CNN-RNN/
│
├── data/
│   └── MNIST dataset
│
├── models/
│   ├── best_cnn_model.pth
│   └── best_rnn_model.pth
│
├── notebook/
│   └── HandWritten_Digit_Classifier.ipynb
│
├── results/
│   ├── cnn_confusion_matrix.png
│   └── rnn_confusion_matrix.png
│
└── README.md