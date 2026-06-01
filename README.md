# Deep Learning Midterm Implementation

This repository contains the implementation work for a Deep Learning midterm assignment covering three tasks:

1. MNIST classifier using manual full-batch gradient descent  
2. Synthetic teacher-student neural network  
3. YOLO-based face detection  

## Project Overview

The goal of this project is to demonstrate different levels of deep learning implementation, starting from manual gradient descent and moving toward practical computer vision using YOLO.

## Question 1: MNIST Classifier Using Manual Full-Batch Gradient Descent

In Question 1, a linear softmax classifier was implemented for MNIST handwritten digit classification. The model was trained using manually derived full-batch gradient descent.

### Key Results

- Validation Accuracy: 87.52%
- Test Accuracy: 89.26%
- Validation Macro F1: 0.8735

## Question 2: Teacher-Student Neural Network

In Question 2, synthetic 2D data was generated using a teacher model. A two-layer neural network was then trained to learn the teacher-generated decision boundary.

### Key Results

- Validation Accuracy: 99.70%
- Validation F1-Score: 0.9970
- Hidden Units: 16
- Epochs: 200

## Question 3: YOLO Face Detection

In Question 3, a YOLO model was adapted for face detection. A pretrained YOLO nano model was used, with most layers frozen and only the final detection head trained for the face class.

### Key Results from CPU Small Run

- Precision: 0.446
- Recall: 0.163
- mAP50: 0.184
- mAP50-95: 0.0892

The YOLO result is reported as a CPU proof-of-concept because GPU quota was not available during the final run.

## Repository Structure

```text
.
├── README.md
├── Deep_Learning_Midterm_Implementation_Report.pdf
├── notebooks/
│   └── dl-midterm.ipynb
├── images/
│   ├── q1_training_curves.png
│   ├── q1_confusion_matrix.png
│   ├── q2_decision_boundary.png
│   └── q3_yolo_metrics.png
└── requirements.txt
