# Deep-Learning-Rock-Paper-Scissors-Gesture-Classification
**Goal**: Build a high-accuracy deep learning system to classify hand gestures (Rock, Paper, Scissors) using Convolutional Neural Networks (CNNs) and Transfer Learning.

Dataset Name: Rock-Paper-Scissors Hand Gesture Dataset

Total Images: 2,925

Rock: 975

Paper: 975

Scissors: 975

Image Resolution: 224 x 224 pixels

Split:
Training: 70% (2,046 images)
Validation: 15% (438 images)

The dataset was balanced and clean, requiring minimal preprocessing.

**Methodology**
Data Print

Resized images to 224×224 pixels.

Normalized pixel values.

Created PyTorch transforms pipeline for uniform input.

**Model Architectures Tested**

Custom CNN (Baseline)

VGG16 (Deep sequence

ResNet50

GoogLeNet (Inception v1) (Efficient multi-scale feature extraction)

**Transfer Learning**

Pre-trained weights on ImageNet.

Fine-tuned classifier layers for this specific task.

**Evaluation Metrics**

Accuracy

Precision

Recall

F1-Score

Confusion Matrix

**Performance Insights**

Winner: GoogLeNet
Achieved highest accuracy (98.41%) while being computationally efficient.
Perfect for real-time deployment on resource-constrained devices.

Transfer Learning Power:
Pre-trained models outperformed the custom CNN by 16-18%, proving the value of leveraging large-scale pre-trained knowledge.

Speed vs. Accuracy Trade-Off:

Custom CNN: Lightweight but less accurate.

GoogLeNet: High accuracy and fast inference.

VGG16: Accurate but large and slower to train.


