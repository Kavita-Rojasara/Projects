# Image Classification Using Transfer Learning with MobileNetV2

## Overview
This project focuses on building an **image classification model** for the **Caltech-101 dataset**, leveraging **transfer learning** with **MobileNetV2**. The Caltech-101 dataset contains images across 101 diverse categories, such as animals, vehicles, musical instruments, and everyday objects. The primary challenge was to handle the limited number of images per category (40–800, with most categories having around 50 images) and train a high-performing model.

## Features
- Utilizes **MobileNetV2**, a pre-trained model on ImageNet, for feature extraction and transfer learning.
- Custom dense layers were added for classification, tailored to the Caltech-101 dataset.
- Employs **fine-tuning** to adapt the pre-trained layers to the specific characteristics of the dataset.
- Includes **data augmentation** (rotations, flips, and zooms) to improve model generalization.
- Implements **class weights** to address class imbalance in the dataset.

## Workflow
1. **Feature Extraction :**
   - Removed MobileNetV2's top classification layers.
   - Added custom dense layers for the Caltech-101 categories.
   - Kept base layers of MobileNetV2 frozen during initial training.

2. **Fine-Tuning :**
   - Unfroze selected layers of MobileNetV2 to adapt the pre-trained model to Caltech-101.

3. **Data Augmentation :**
   - Applied techniques like rotation, flipping, and zooming to increase the diversity of training data.

4. **Class Weights :**
   - Introduced class weights to handle imbalanced categories and ensure fair training across all classes.

5. **Evaluation :**
   - Evaluated performance using accuracy metrics, a confusion matrix, and a classification report to analyze strengths and weaknesses across categories.

## Dataset
The **Caltech-101 dataset :**
- Contains images across 101 categories.
- Each category includes 40–800 images (most categories have ~50).
- Diverse categories include animals, vehicles, and objects, posing a challenge for classification due to limited data.

## Technologies Used
- **Python :** Core programming language.
- **TensorFlow** and **Keras :** Frameworks for implementing and fine-tuning the MobileNetV2 model.
- **Matplotlib** and **Seaborn :** For visualizing performance metrics like confusion matrices.
- **NumPy** and **Pandas :** For data preprocessing and analysis.
