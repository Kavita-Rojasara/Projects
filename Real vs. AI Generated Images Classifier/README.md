# REAL vs. AI-Generated Images Classifier

## Overview
This project tackles the challenge of distinguishing real images from AI-generated synthetic images using the **CIFAKE dataset**. By leveraging **convolutional neural networks (CNNs)** and **transfer learning** with **ResNet50**, the classifier provides accurate predictions, showcasing its potential in media forensics and content verification.

## Features
- Implements **ResNet50** for transfer learning to enhance classification accuracy.
- Processes 120,000 images from the CIFAKE dataset (real and synthetic images).
- Integrates robust data preprocessing and augmentation techniques for better generalization.
- Provides performance metrics, including confusion matrices, precision-recall scores, and accuracy.

## Technologies Used
- **Python :** Primary programming language.
- **TensorFlow** and **Keras :** Frameworks for implementing and training CNNs.
- **OpenCV :** For image preprocessing and augmentation.
- **Matplotlib** and **Seaborn :** For data visualization and performance metrics.

## Use Cases
- **Media Forensics :** Detects AI-generated content to ensure authenticity.
- **Content Moderation :** Identifies synthetic images for digital platforms.
- **Image Authentication :** Validates image authenticity for secure applications.
