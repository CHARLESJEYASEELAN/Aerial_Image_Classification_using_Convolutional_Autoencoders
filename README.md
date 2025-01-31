# **Aerial Image Classification using Convolutional Autoencoders**

## **Project Overview**
This project aims to classify aerial images into four categories (**Agriculture, Airport, Beach, and City**) using **Convolutional Autoencoders (CAEs)** for feature extraction and ANN based classification. The model achieved an Test Accuracy of **84%**.

## **Dataset**
The dataset consists of aerial images labeled into four classes:

- 🌾 **Agriculture**  
- 🏙 **City**  
- 🏖 **Beach**  
- ✈ **Airport**  

## **Methodology**
### **1. Data Preprocessing**
- Resizing images to a standard dimension. (224,224)
- Normalization to scale pixel values between 0 and 1.

### **2. Feature Extraction with Convolutional Autoencoders**
- The **encoder** compresses the image into a lower-dimensional latent space representation.
- The **decoder** reconstructs the original image from this compressed representation.
- This unsupervised learning approach helps in efficient feature extraction.

### **3. Classification**
- The latent space representations from the encoder were used as input features for a classifier.
- A **fully connected neural network** was trained on these extracted features.

### **4. Evaluation**
- Achieved an accuracy of **84%**, demonstrating the effectiveness of autoencoders in aerial image classification.

## **Results & Observations**
- The model effectively learned **spatial patterns** in aerial imagery.
- Autoencoder-based feature extraction helped in **reducing computational complexity**.
- Further tuning of hyperparameters and network depth may **improve performance**.

## **Technologies Used**
- 🐍 Python
- 🔬 TensorFlow/Keras
- 🖼 OpenCV
- 📊 NumPy & Pandas
- 📉 Matplotlib & Seaborn

## **Future Improvements**
- Implement **attention mechanisms** for better feature selection.
- Experiment with **transfer learning** using pretrained models like ResNet.
- Extend to **multi-label classification** for more complex aerial scene analysis.

