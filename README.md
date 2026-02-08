# Edge AI based Wafer Defect Detection

## Problem Statement
Automated detection and classification of semiconductor manufacturing defects
from wafer inspection images, optimized for edge deployment.

## Defect Classes
- Clean
- Shorts
- Opens
- Bridges
- Cracks
- Malformed Vias
- Other

## Dataset
- Custom dataset collected from publicly available wafer defect image sources
- Images converted to grayscale to reduce model size and improve edge performance
- Dataset split into Train, Validation, and Test folders
- Folder-based class labeling using ImageFolder

## Model Architecture
- Convolutional Neural Network (CNN)
- Supervised learning approach
- Lightweight architecture designed for edge devices
- Input: 96x96 grayscale images

## Training Details
- Framework: PyTorch
- Loss Function: CrossEntropyLoss
- Optimizer: Adam
- Epochs: 15
- Platform: Google Colab (T4 GPU)

## Evaluation Metrics
- Accuracy
- Precision
- Recall
- Confusion Matrix

Sample Results:
- Accuracy: 41.46%
- Precision: 40.99%
- Recall: 41.46%

## Model Export
- All experiments and training were performed using Google Colab with GPU acceleration.
- Trained model exported to ONNX format
- ONNX model compatible with NXP eIQ toolchain

## Files Description
- train.py : Model training script
- evaluate.py : Model evaluation and metrics
- export_onnx.py : ONNX model export
- inference.py : Inference script
- requirements.txt : Required dependencies

## Future Improvements
- Class imbalance handling
- Data augmentation
- Transfer learning
- Edge-specific optimization using NXP eIQ

## Hackathon
IESA DeepTech Hackathon – Phase 1 Submission
