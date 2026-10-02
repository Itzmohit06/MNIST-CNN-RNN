# Handwritten Digit Classification using CNN and RNN

This project focuses on handwritten digit classification using the **MNIST dataset**. Two different deep learning approaches, **CNN and RNN**, were implemented and evaluated on the same dataset.

The main goal was to understand how both models perform for handwritten digit recognition and compare their results.

## Dataset

The project uses the MNIST handwritten digit dataset.

- Training images: 60,000
- Test images: 10,000
- Image size: 28 × 28 pixels
- Classes: 10 (digits 0–9)

The original training data was divided into:

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

## CNN Model

The CNN model uses convolutional layers, ReLU activation, max pooling, and fully connected layers to learn spatial features from handwritten digit images.

**CNN Test Accuracy: 98.90%**

## RNN Model

For the RNN, each 28 × 28 image was treated as a sequence of 28 rows, with each row containing 28 features.

### Original RNN

The original RNN achieved:

**Test Accuracy: 93.66%**

### Improved RNN

The RNN was improved by:

- Increasing the number of RNN layers from 1 to 2
- Using bidirectional processing
- Adding dropout
- Using the AdamW optimizer
- Increasing the learning rate
- Increasing training epochs
- Using gradient clipping for stable training

After these changes:

**Improved RNN Test Accuracy: 96.52%**

The RNN accuracy improved from **93.66% to 96.52%**.

## Final Results

| Model | Test Accuracy |
|---|---:|
| CNN | **98.90%** |
| Original RNN | **93.66%** |
| Improved RNN | **96.52%** |

### Final Selected Model

Based on the final test results, the **CNN was selected as the final model**.

**Selected Model:** CNN  
**Final Test Accuracy:** **98.90%**

The CNN achieved higher test accuracy than the improved RNN on the same MNIST test dataset.

## Results

Confusion matrices were generated to analyze the predictions of the models.

The results are available in the `results/` folder.

## What I Learned

Through this project, I learned:

- How to prepare the MNIST dataset for deep learning.
- How CNNs can be used for image classification.
- How images can be represented as sequences for an RNN.
- How to train and evaluate models using PyTorch.
- How model architecture and training parameters affect performance.
- How to use confusion matrices for classification analysis.
- How to compare different deep learning models using the same dataset.

## Project Structure

```text
MNIST-CNN-RNN/
│
├── data/
├── models/
├── notebook/
│   └── HandWritten_Digit_Classifier.ipynb
├── results/
└── README.md
```

## Conclusion

Both CNN and RNN models successfully classified handwritten digits.

The **CNN achieved 98.90% accuracy**, while the **improved RNN achieved 96.52%**. The RNN also showed an improvement from its original accuracy of **93.66%**.

Based on the final test results, **CNN was selected as the final model with 98.90% test accuracy**.

## Author

**Mohit Chavan**  
B.Tech - Artificial Intelligence and Machine Learning  

GitHub: [Itzmohit06](https://github.com/Itzmohit06)