# 🧠 Violence Detection in Videos using Deep Learning

A deep learning system that automatically classifies video frames as **Violence** or **Non-Violence** using CNN-based models.

## 📊 Dataset

**Source:** [Real-Life Violence Dataset](https://www.kaggle.com/datasets/karandeep98/real-life-violence-and-nonviolence-data)
- 11,063 frames (8,851 train / 2,212 val)
- Binary classification: Violence vs Non-Violence
- Image size: 224×224 pixel

## 🚀 Models & Results

| Model | Val Accuracy | Val Loss | Speed |
|-------|-------------|----------|-------|
| Custom CNN | 68.40% | 0.58 | Fast |
| **ResNet50** | **94.17%** | 0.17 | Moderate |
| **MobileNetV2** | **93.31%** | 0.18 | Fastest |

## ✨ Features

- **Advanced Preprocessing:** CLAHE, brightness/contrast adjustment, normalization
- **Transfer Learning:** ResNet50 & MobileNetV2 with ImageNet weights
- **Two-Stage Fine-Tuning:** Freeze → Unfreeze top layers with reduced LR
- **Data Augmentation:** Rotation, zoom, horizontal flip
- **Callbacks:** ModelCheckpoint, EarlyStopping

## 🛠️ Installation
```bash
git clone https://github.com/yourusername/violence-detection.git
cd violence-detection
pip install -r requirements.txt
```

