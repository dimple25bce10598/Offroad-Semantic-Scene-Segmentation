# Offroad-Semantic-Scene-Segmentation
# Project Overview

Implements a deep learning–based semantic scene segmentation pipeline for off-road environments

Focuses on pixel-level classification of complex terrain and object categories

Designed to support off-road autonomy and unmanned ground vehicle (UGV) perception

Trained exclusively on synthetic desert datasets generated using digital twin simulation

Evaluated on unseen environments to measure robustness and generalization

# Objectives

Perform accurate pixel-wise classification of off-road scenes

Segment terrain elements such as vegetation, rocks, ground clutter, landscape, and sky

Build a model that generalizes well under domain shift conditions

Ensure strict separation of training, validation, and test datasets

Provide a reproducible and well-documented implementation

# Dataset Description

Consists of synthetic RGB images and corresponding segmentation masks

Each pixel in the mask is assigned a predefined semantic class

Dataset is organized to prevent data leakage during training

Dataset Structure
dataset/
 ├── train/
 │    ├── images/
 │    └── masks/
 ├── val/
 │    ├── images/
 │    └── masks/
 └── testImages/

Training and validation data are used only for model learning

Test images are reserved strictly for final evaluation

# Model & Approach

Uses a fully convolutional neural network (FCN)–based segmentation model

Learns spatial and contextual features required for off-road scene understanding

Supports multi-class semantic segmentation

Designed for scalability and further optimization

# Technology Stack

Python

PyTorch

OpenCV

NumPy

Matplotlib

Visual Studio Code

# Environment Setup

Create a Python virtual environment for dependency isolation

Install required packages using requirements.txt

Fully compatible with local development using VS Code

# Model Training

Training is performed using the provided train.py script

Loads images and corresponding segmentation masks

Optimizes the model using cross-entropy loss

Saves trained model weights for later evaluation

# Testing & Evaluation

Testing is performed using the test.py script

Evaluates the model on unseen test images

Generates predicted segmentation masks

Provides qualitative and quantitative performance insights

# Evaluation Metrics

Intersection over Union (IoU) for segmentation accuracy

Training loss across epochs

Visual comparison between ground truth and predicted masks

# Repository Structure
├── README.md
├── Test.py
├── Train.py
├── predictions
# Reproducibility & Best Practices

No test data is used during training or validation

Clear dataset separation is strictly maintained

All experiments are reproducible using the provided scripts

Code and structure follow hackathon evaluation guidelines

# Applications

Off-road autonomous navigation

Perception systems for unmanned ground vehicles

Research on synthetic data–driven computer vision

Semantic understanding of unstructured environments

# Usage & License

Intended for educational, research, and hackathon purposes

Can be extended for advanced segmentation research

# Final Results
Final Val Loss: 0.8161
Final Val IoU: 0.2932
Final Val Dice: 0.4372
Final Val Accuracy: 0.7023

