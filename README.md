# Kubernetes Intrusion Detection System

## Project Overview

This project implements a neural network-based intrusion detection system (IDS) for Kubernetes environments using deep learning techniques. The system is designed to detect various types of cyber attacks in containerized Kubernetes applications by analyzing network traffic patterns.

The model is built using TensorFlow/Keras and optimized using Optuna for hyperparameter tuning, achieving high accuracy in classifying normal and malicious traffic.

## Dataset

The project uses the [Kube-IDS0 dataset](https://www.kaggle.com/datasets/redamorsli/kube-ids0), which includes two intrusion detection datasets collected on a K8s cluster. The datasets were collected by simulating normal and malicious activities on two different web apps hosted on the cluster.

## Features

- Data preprocessing pipeline for network traffic features
- Hyperparameter optimization using Optuna
- Neural network architecture with configurable layers and dropout
- High accuracy classification of attack vs. normal traffic
- Model evaluation and persistence

## Requirements

- Python 3.8+
- TensorFlow 2.x
- Pandas
- NumPy
- Optuna
- Scikit-learn

## Model Architecture

The final model is a feed-forward neural network with:
- Input layer matching the feature dimensions
- Two hidden layers with ReLU activation
- Dropout layers to prevent overfitting
- Output layer with softmax activation for multi-class classification

## Performance

The final model achieves approximately 100% accuracy on the test set, demonstrating excellent performance in distinguishing between normal and malicious traffic patterns.

## Contributors

Team Name: codersincrocs

- Sri Vidya (Team Lead)
- Surya P S
- Siri N Shetty
- Suprith S