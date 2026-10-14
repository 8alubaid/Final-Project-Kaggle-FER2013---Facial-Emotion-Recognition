# SDAIA Academy - FER2013 Facial Emotion Recognition / Instructor: Rand Bernawi

This project compares three deep learning approaches for facial emotion recognition using the FER2013 dataset:

- Custom CNN
- EfficientNet-B0 Transfer Learning
- EfficientNet-B0 Partial Fine-Tuning

## Dataset

FER2013 contains 48×48 grayscale facial images classified into 7 emotions:

- Angry
- Disgust
- Fear
- Happy
- Neutral
- Sad
- Surprise

## Models

### 1. Custom CNN
A CNN built from scratch with convolutional layers, Batch Normalization, Max Pooling, and Dropout.

Final Test Accuracy: **58.80%**

### 2. EfficientNet-B0 Transfer Learning
A pretrained EfficientNet-B0 model with the feature extractor frozen and only the classifier trained on FER2013.

Final Test Accuracy: **44.22%**

### 3. EfficientNet-B0 Partial Fine-Tuning
The last EfficientNet feature blocks and classifier were trained to better adapt the pretrained model to FER2013.

Final Test Accuracy: **53.46%**

## Results

| Model | Test Accuracy |
|---|---:|
| Custom CNN | 58.80% |
| EfficientNet-B0 Transfer Learning | 44.22% |
| EfficientNet-B0 Partial Fine-Tuning | 53.46% |

The Custom CNN achieved the highest test accuracy in this experiment.

## Technologies

- Python
- PyTorch
- Torchvision
- EfficientNet-B0
- Matplotlib
- Scikit-learn
- Google Colab
