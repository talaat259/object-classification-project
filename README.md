# 🚗 Car Detection using Deep Neural Network

This project implements a deep convolutional neural network (CNN) to detect and classify cars from images as part of a Big Data project. The architecture combines multiple convolutional layers followed by dense layers with dropout for regularization.

---

## 🧠 Model Summary

| Layer (type)                 | Output Shape        | Param #     |
|-----------------------------|---------------------|-------------|
| conv2d_18 (Conv2D)          | (None, 125, 125, 32)| 320         |
| conv2d_19 (Conv2D)          | (None, 125, 125, 16)| 4,624       |
| conv2d_20 (Conv2D)          | (None, 125, 125, 4) | 580         |
| conv2d_21 (Conv2D)          | (None, 125, 125, 16)| 592         |
| conv2d_22 (Conv2D)          | (None, 125, 125, 4) | 580         |
| conv2d_23 (Conv2D)          | (None, 125, 125, 16)| 592         |
| conv2d_24 (Conv2D)          | (None, 125, 125, 4) | 580         |
| conv2d_25 (Conv2D)          | (None, 125, 125, 16)| 592         |
| conv2d_26 (Conv2D)          | (None, 125, 125, 4) | 68          |
| max_pooling2d_2             | (None, 17, 17, 4)   | 0           |
| flatten_2                   | (None, 1156)        | 0           |
| layer1 (Dense)              | (None, 256)         | 296,192     |
| dropout_18 (Dropout)        | (None, 256)         | 0           |
| layer2 (Dense)              | (None, 256)         | 65,792      |
| dropout_19 (Dropout)        | (None, 256)         | 0           |
| layer3 (Dense)              | (None, 256)         | 65,792      |
| dropout_20 (Dropout)        | (None, 256)         | 0           |
| layer4 (Dense)              | (None, 128)         | 32,896      |
| dropout_21 (Dropout)        | (None, 128)         | 0           |
| layer5 (Dense)              | (None, 128)         | 16,512      |
| layer32 (Dense)             | (None, 128)         | 16,512      |
| dropout_22 (Dropout)        | (None, 128)         | 0           |
| dense_9 (Dense)             | (None, 128)         | 16,512      |
| dropout_23 (Dropout)        | (None, 128)         | 0           |
| dense_10 (Dense)            | (None, 128)         | 16,512      |
| dropout_24 (Dropout)        | (None, 128)         | 0           |
| dense_11 (Dense)            | (None, 64)          | 8,256       |
| dropout_25 (Dropout)        | (None, 64)          | 0           |
| dense_12 (Dense)            | (None, 64)          | 4,160       |
| dense_13 (Dense)            | (None, 32)          | 2,080       |
| dropout_26 (Dropout)        | (None, 32)          | 0           |
| dense_14 (Dense)            | (None, 32)          | 1,056       |
| dropout_27 (Dropout)        | (None, 32)          | 0           |
| dense_15 (Dense)            | (None, 16)          | 528         |
| dropout_28 (Dropout)        | (None, 16)          | 0           |
| layer6 (Dense)              | (None, 16)          | 272         |
| layer7 (Dense)              | (None, 8)           | 136         |
| output (Dense)              | (None, 5)           | 45          |
| reshape_2 (Reshape)         | (None, 5, 1)        | 0           |

---

## 📊 Performance

| Metric       | Value       |
|--------------|-------------|
| **Loss**     | `2.38e-08`  |
| **Accuracy** | `88.19%`    |

---

## 📦 Model Details

- **Total Parameters**: `1,655,345` (~6.31 MB)
- **Trainable Parameters**: `551,781` (~2.10 MB)
- **Optimizer Parameters**: `1,103,564` (~4.21 MB)

---
