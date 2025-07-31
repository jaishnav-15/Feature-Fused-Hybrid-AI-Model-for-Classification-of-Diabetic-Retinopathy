# Feature-Fused-Hybrid-AI-Model-for-Classification-of-Diabetic-Retinopathy
Overview
This repository contains the implementation of a novel and robust hybrid AI model for the precise, multi-grade classification of Diabetic Retinopathy (DR) from retinal fundus images. Diabetic Retinopathy is a leading cause of vision impairment and blindness worldwide. Timely and accurate diagnosis is essential to prevent permanent vision loss, but manual detection by ophthalmologists is time-consuming, subjective, and prone to errors.

Our proposed system addresses these limitations by combining the power of deep learning for comprehensive feature extraction with the efficiency and interpretability of machine learning for final diagnosis. The model processes retinal fundus images, classifies them into five DR grades (No DR, Mild, Moderate, Severe, and Proliferative), and provides a reliable tool for early intervention.

# Key Features

Hybrid AI Architecture: Integrates state-of-the-art deep learning models (EfficientNet-B3, ResNet-50, DenseNet-121) for feature extraction with an XGBoost classifier for final diagnosis.


Advanced Image Preprocessing: Employs crucial preprocessing techniques such as CLAHE (Contrast Limited Adaptive Histogram Equalization) for contrast enhancement, Gaussian blurring for noise reduction, and grayscale conversion to optimize image quality and standardize input dimensions.


Multi-Model Feature Fusion: Features extracted from the three distinct CNN architectures are concatenated to create a comprehensive "feature-fused vector" (4608-D), capturing diverse image representations and mitigating individual model limitations.


Robustness through Test-Time Augmentation (TTA): Implements TTA during inference by generating multiple augmented versions (horizontal flips, slight rotations up to +15°, and brightness changes) of test images and averaging their outputs for more stable and consistent predictions.

High Performance: Achieves an impressive overall accuracy of 96.49% on the validation set, demonstrating superior diagnostic capabilities across all five DR grades.


Detailed Evaluation: Comprehensive performance metrics, including accuracy, precision, recall, F1-score, confusion matrices, and ROC-AUC curves, are provided, showcasing balanced performance and high discriminative power.

Clinical Relevance: Automates DR screening to reduce diagnostic time, human error, and subjectivity, enabling earlier intervention to prevent vision loss in diabetic patients. The model is designed for scalability and adaptability in clinical and telemedicine applications.


