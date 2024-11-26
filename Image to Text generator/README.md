# **Image to Text Generator Using Vision Transformers and GPT-2**

## Overview
This project implements an **Image to Text Generator** leveraging **Vision Transformers (ViT)** for image feature extraction and **GPT-2** for generating descriptive captions. The model processes images and outputs meaningful, contextually relevant captions, showcasing the power of combining computer vision and natural language processing.

## Features
- Uses **Vision Transformers (ViT)** for robust image feature extraction.
- Generates descriptive and coherent captions using **GPT-2**.
- Supports batch processing for handling multiple images efficiently.
- Modular and scalable architecture for further extensions and customization.

## How It Works 
- **Image Feature extraction :** Vision Transformers (ViT) preprocess and encode images into a high-dimensional feature vector.
- **Text Generation :** GPT-2 takes the feature vector and generates a coherent and meaningful caption.
- **End-to-End Pipeline :** The entire process is streamlined into a single pipeline for ease of use and deployment.

## Technologies Used
- **Python :** Primary programming language for development.
- **Hugging Face Transformers :** Pre-trained models for Vision Transformers and GPT-2.
- **PyTorch :** Deep learning framework for training and inference.
- **OpenCV :** For image preprocessing and handling.
- **NumPy :** For efficient numerical computations.

## Use Cases
- **Accessibility :** Helps visually impaired individuals understand visual content through text descriptions.
- **E-commerce :** Automates product descriptions for online stores.
- **Content Creation :** Assists in generating captions for social media platforms.
- **Media Automation :** Enables automatic tagging and metadata generation.

