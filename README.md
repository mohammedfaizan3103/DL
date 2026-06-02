# Deep Learning Techniques for Sign Language Recognition

## Overview

This project presents a comprehensive experimental study of deep learning techniques for Sign Language Recognition using the Sign Language MNIST dataset. Multiple neural network architectures, optimization strategies, regularization techniques, and model interpretability methods are evaluated and compared.

The objective is to analyze how different deep learning approaches perform on hand gesture classification and identify the most effective architectures for low-resolution image recognition tasks.

## Features

* Multi-Layer Perceptron (MLP) experiments
* Learning Rate and Epoch Analysis
* Gradient Descent Variant Comparison
* Regularization Techniques

  * L2 Regularization
  * Data Augmentation
  * Early Stopping
  * Dropout
  * Noise Injection
* Custom Convolutional Neural Networks (CNNs)
* Classical Deep Learning Architectures

  * LeNet-5
  * AlexNet
  * ZFNet
  * VGGNet
  * GoogLeNet
  * ResNet
* Autoencoder-based Representation Learning
* CNN Feature Map Visualization
* Guided Backpropagation for Model Interpretability

## Dataset

The project uses the Sign Language MNIST dataset containing grayscale images of American Sign Language alphabet gestures.

* Image Size: 28 × 28
* Classes: 26 alphabet classes
* Training Samples: ~27,455
* Format: Grayscale images

Dataset Source:
https://www.kaggle.com/datamunge/sign-language-mnist

## Key Results

| Model                        | Accuracy                 |
| ---------------------------- | ------------------------ |
| MLP (Best Configuration)     | 99.98%                   |
| Custom CNN                   | 99%+                     |
| LeNet-5                      | 99%+                     |
| ResNet                       | 100% Validation Accuracy |
| Autoencoder (256-D Encoding) | Excellent Reconstruction |

### Major Findings

* CNNs significantly outperform traditional MLPs for image classification.
* Learning rates above 0.001 cause MLP training instability.
* Dropout (0.2) provides the best regularization performance.
* LeNet-5 is highly effective for low-resolution sign language images.
* ResNet benefits from residual connections and converges rapidly.
* Large architectures such as AlexNet and VGGNet are unsuitable for heavily upscaled low-resolution inputs.

## Technologies Used

* Python
* TensorFlow
* Keras
* NumPy
* Matplotlib
* Scikit-learn
* OpenCV

## Project Structure

```text
├── notebooks/
│   └── DL_Lab.ipynb
├── models/
├── visualizations/
├── results/
├── report/
└── README.md
```

## Future Improvements

* Real-time sign language recognition
* Transfer learning with domain-specific datasets
* Transformer-based architectures
* Video-based gesture recognition
* LSTM and Temporal Modeling
* Multi-hand gesture recognition

