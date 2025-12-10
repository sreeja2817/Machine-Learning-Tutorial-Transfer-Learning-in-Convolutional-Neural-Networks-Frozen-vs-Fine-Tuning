# Machine-Learning-Tutorial-Transfer-Learning-in-Convolutional-Neural-Networks-Frozen-vs-Fine-Tuning
7PAM2021-0901-2025 - Machine Learning Tutorial

# Transfer Learning in CNNs: Frozen vs Fine-Tuning (MobileNetV2)

Author: Sreeja Nalla  
Student ID: 24088662  

## Project Overview
This project compares three approaches to image classification using a flower dataset:

1. Baseline CNN trained from scratch
2. Transfer learning with a frozen MobileNetV2 backbone
3. Transfer learning with fine-tuning of the upper layers

The goal is to demonstrate the impact of transfer learning and fine-tuning on classification performance.

## Dataset
Flowers Recognition Dataset from Kaggle:  
https://www.kaggle.com/datasets/alxmamaev/flowers-recognition

Classes:
- Daisy
- Dandelion
- Rose
- Sunflower
- Tulip

Learning Objectives

--By completing this project, you will understand:

--How CNNs learn image features from scratch

--Why training deep networks on small datasets fails

--How frozen transfer learning works

--When fine-tuning provides additional benefit

--How pretrained models improve performance

--How to analyse confusion matrices and learning curves

Models Implemented
🔹 Baseline CNN (From Scratch)

A manually designed CNN with three convolution blocks and a dense classifier.

Key Findings:

Overfits quickly

Struggles with generalisation

Accuracy ≈ 67%

🔹 MobileNetV2 (Frozen Feature Extractor)

MobileNetV2 pretrained on ImageNet is loaded and frozen.
Only the classifier head is trained.

Advantages:

Faster convergence

Lower overfitting

Smaller trainable parameter count

Accuracy: ~88%

🔹 MobileNetV2 (Fine-Tuned)

Final layers are unfrozen and retrained using a low learning rate.

Advantages:

Learns flower-specific patterns

Improves discriminative power

Best performance across all experiments

Accuracy: ~91%

▶ How To Run

Download the dataset ZIP file

Open and run the notebook from start to end

Dataset is automatically extracted

Data is cleaned and prepared

Baseline CNN is trained

Transfer learning model is applied

Fine-tuning is performed

Accuracy plots, confusion matrices and predictions are generated
