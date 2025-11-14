# EfficientNet-vs-ResNet-A-comprehensive-comparison-on-multi-class-classification
comparison of efficientNet and ResNet on Intel image classification dataset (multi-class) using pytorch .

## Overview
* End-to-end comparison of EfficientNet-B0 and ResNet50 on the Intel Image Classification dataset.
* Both models trained under identical conditions for a fair architectural evaluation.
* Focused on accuracy, efficiency, speed, and interpretability using Grad-CAM.

## Objectives
* Compare two popular CNN architectures on the same dataset.
* Measure training/validation accuracy and loss.
* Evaluate parameter count and inference speed.
* Plot learning curves for clearer insights.
* Generate Grad-CAM heatmaps for model interpretability.

## Model Details

### EfficientNet-B0
* ~5.3M parameters
* Lightweight and fast
* Performs extremely well on small/medium datasets

### ResNet50
* ~25M parameters
* Much deeper architecture
* Requires more compute and tends to overfit on limited data

## What Was Compared
* Training Accuracy
* Validation Accuracy
* Training Loss
* Validation Loss
* Parameter Count
* Training Time per Epoch
* Inference Speed
* Grad-CAM Visualization Quality

## Plotting Comparison
* Accuracy curves show how each model generalizes across epochs.
* Loss curves highlight how stable and consistent the learning process is.
* EfficientNet-B0 maintains steadier validation performance than ResNet50.

## Findings
* EfficientNet-B0 achieved higher validation accuracy than ResNet50.
* ResNet50 showed stronger signs of overfitting.
* EfficientNet-B0 trained faster per epoch.
* EfficientNet-B0 used far fewer parameters.
* Grad-CAM outputs from EfficientNet-B0 were more focused and localized.

## Grad-CAM Insights
* Side-by-side Grad-CAM visualizations were generated for both models.
* EfficientNet-B0 highlighted more meaningful image regions.
* ResNet50 showed more diffused attention in several test cases.

## Tech Stack
* PyTorch
* Torchvision
* NumPy
* OpenCV
* PIL
* Matplotlib

## Conclusion
* EfficientNet-B0 is the more suitable model for small-to-medium datasets.
* It offers faster training, better generalization, and lower computational cost.
* ResNet50 remains a strong baseline but needs more data to shine.
* This project demonstrates strong in training, evaluation, visualization, and model interpretability.
