# 🎨 Colorize-It: Deep Learning for Automatic Image Colorization

This project uses a deep learning model to **automatically add color to grayscale images**, bringing them to life. Built using Convolutional Neural Networks (CNNs), the model learns from thousands of color images and learns to predict RGB values for grayscale input.

---

## 🧠 Project Overview

- Converts black-and-white (grayscale) images into realistic colored versions.
- Trained on a large dataset of natural images.
- Uses a deep CNN to learn pixel-wise color mapping.
- Ideal for restoring old photos, artistic image generation, or AI-based photo editing.

---

## 🛠️ Tech Stack

- **Language:** Python 3.10+
- **Framework:** TensorFlow / Keras or PyTorch
- **Libraries:** OpenCV, NumPy, Matplotlib, Scikit-learn
- **Notebook:** Jupyter / Colab for training and demo

---

## 🗂️ Dataset

- **Dataset Used:** [Places365](http://places.csail.mit.edu/) or [ImageNet subset]
- Images were converted to **Lab color space** for better separation of luminance and chrominance channels.
- Only the **L (grayscale)** channel is input to the model; **a & b (color)** channels are predicted.

---

## 🔧 How It Works

1. Convert color images to Lab format.
2. Use the **L channel** as input; model predicts **a and b channels**.
3. Concatenate L, a, b → convert back to RGB for final color image.

