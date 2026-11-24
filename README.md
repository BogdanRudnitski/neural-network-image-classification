# Neural Network Image Classification

Academic machine learning project for **COMP 551 - Applied Machine Learning** at McGill University.

Implemented and evaluated multilayer perceptrons, convolutional neural networks, and transfer learning models for image classification using Fashion-MNIST and CIFAR-10.

## Project Overview

- **Multilayer Perceptron:** Implemented an MLP from scratch using NumPy, backpropagation, mini-batch gradient descent, and L1/L2 regularization.
- **Model Experiments:** Studied network depth and width, activation functions, regularization strength, input normalization, and data augmentation.
- **Convolutional Neural Network:** Built a PyTorch CNN and evaluated augmentation using five random seeds.
- **Transfer Learning:** Used ResNet18 pre-trained on ImageNet, keeping its original layers frozen and training new fully connected layers on Fashion-MNIST and CIFAR-10.

## Results

- **88.97% test accuracy** using the best L2-regularized MLP on Fashion-MNIST.
- **90.44% mean test accuracy** for the Fashion-MNIST CNN without augmentation, increasing to **90.90% with augmentation** across five seeds (standard deviations of 0.30 and 0.33 percentage points, respectively).
- **75.22% test accuracy** using frozen ResNet18 with augmentation on CIFAR-10, compared with **67.12%** for the CNN trained from scratch.
- Augmentation improved the CNN's mean accuracy on Fashion-MNIST but reduced accuracy for the MLP configurations tested.

## Technologies

Python, NumPy, Matplotlib, PyTorch, torchvision, Jupyter Notebook

## Files

- [Multilayer Perceptron Notebook](multilayer_perceptron.ipynb) – NumPy implementation, experiments, and visualizations.
- [Convolutional Neural Network Notebook](convolutional_neural_network.ipynb) – CNN experiments and ResNet18 transfer learning.
- [Project Report](report.pdf) – Methodology, results, and discussion.
- [Requirements](requirements.txt) – Python dependencies.

## Contributors

Bogdan Rudnitski, Olivier Ren, Maxim Qu
