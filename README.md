# Malaria Parasite Detection using CNN

## Project Overview

This project implements a **Convolutional Neural Network (CNN)** to automatically detect malaria parasites in microscopic blood smear images. The model classifies images into two categories: **Parasitised (infected)** and **Uninfected (healthy)** red blood cells.

Malaria diagnosis is traditionally performed by manually examining blood smear slides under a microscope. This process is time-consuming and depends on expert analysis. The proposed deep learning model helps automate the detection process and supports faster medical screening.

---

## Dataset

The dataset used for this project contains microscopic images of red blood cells.

**Classes**

* Parasitised (Infected cells)
* Uninfected (Healthy cells)

**Dataset Details**

* Training Images: ~13,990
* Validation Images: ~3,496
* Image Size: 48 × 48 pixels
* Source: Malaria Cell Images Dataset (NIH / Kaggle)

---

## Technologies Used

* Python
* TensorFlow / Keras
* NumPy
* Matplotlib
* Google Colab / Jupyter Notebook

---

## Model Architecture

The Convolutional Neural Network consists of the following layers:

1. **Conv2D Layer** – 32 filters, kernel size (3×3), ReLU activation
2. **MaxPooling Layer** – (2×2)
3. **Conv2D Layer** – 64 filters, kernel size (3×3), ReLU activation
4. **MaxPooling Layer** – (2×2)
5. **Flatten Layer** – converts feature maps into a vector
6. **Dense Layer** – 64 neurons with ReLU activation
7. **Output Layer** – 1 neuron with Sigmoid activation

**Loss Function:** Binary Crossentropy
**Optimizer:** Adam

---

## Training Process

1. Load dataset and preprocess images.
2. Normalize pixel values.
3. Split dataset into training and validation sets.
4. Train the CNN model for multiple epochs.
5. Evaluate model performance using accuracy and loss metrics.

---

## Results

Model performance during training:

* Training Accuracy: ~98%
* Validation Accuracy: ~88.7%
* Final Validation Loss: ~0.30

Training graphs show improvement in accuracy and reduction in loss as epochs increase.

---

## Project Structure

```
Malaria-Detection-CNN/
│
├── Malaria Parasite DetectionCNN.ipynb
├── README.md
├── malaria_detection_full_report.pdf
└── dataset/
```

---

## How to Run the Project

1. Open the notebook in Google Colab
2. Mount Google Drive
3. Load the dataset
4. Run all cells in the notebook
5. Train and evaluate the model
```

3. Open the notebook

```
Malaria Parasite DetectionCNN.ipynb
```

4. Run all cells to train the model.

---

## Future Improvements

* Apply **transfer learning** using models such as ResNet or MobileNet.
* Increase dataset size to improve model generalization.
* Develop a **web or mobile application** for real-time malaria detection.
* Implement visualization techniques like Grad-CAM to explain model predictions.

---

## Conclusion

The CNN-based malaria detection system demonstrates that deep learning can assist in medical image analysis. Automated detection can support healthcare professionals by providing faster and more consistent malaria diagnosis.
‎README.md‎
+123
Lines changed: 123 additions & 0 deletions


Original file line number	Diff line number	Diff line change
@@ -1,2 +1,125 @@
# SoftGrowTech_Project3_Malaria-Detection-ML
Malaria Parasite Detection using CNN on microscopic blood cell images
# Malaria Parasite Detection using Convolutional Neural Networks (CNN)
## Project Overview
This project implements a Machine Learning model to detect malaria parasites from microscopic blood smear images. The system uses a Convolutional Neural Network (CNN) to classify blood cell images into two categories: **Parasitised** (infected) and **Uninfected** (healthy).
Early detection of malaria is important for effective treatment. This project demonstrates how Artificial Intelligence can assist healthcare professionals in diagnosing malaria using image classification techniques.
---
## Dataset
The dataset consists of microscopic images of blood cells divided into two classes:
* **Parasitised** – Blood cells infected with malaria parasites
* **Uninfected** – Healthy blood cells
Total images in dataset: **~27,000**
The dataset was used to train and evaluate the CNN model.
---
## Technologies Used
* Python
* TensorFlow / Keras
* NumPy
* Matplotlib
* Scikit-learn
* Google Colab
---
## Model Architecture
The Convolutional Neural Network (CNN) used in this project consists of:
* Convolution Layers for feature extraction
* MaxPooling Layers for dimensionality reduction
* Flatten Layer to convert feature maps into vectors
* Dense Layers for classification
* Sigmoid Output Layer for binary classification
---
## Project Workflow
1. Load dataset from Google Drive
2. Preprocess and normalize image data
3. Split dataset into training and validation sets
4. Build CNN model architecture
5. Train the model using training data
6. Evaluate model performance
7. Plot training accuracy and loss graphs
8. Save the trained model
---
## Results
Model Performance:
* Training Accuracy: **~93% – 95%**
* Validation Accuracy: **~92% – 94%**
Training graphs show decreasing loss and increasing accuracy during model training.
---
## Project Structure
Malaria-Detection-ML/
dataset/
Contains parasitised and uninfected blood cell images
notebook/
Contains the Google Colab notebook used to train the model
model/
Contains the trained CNN model file
results/
Contains accuracy and loss graphs generated during training
documentation/
Contains project report and supporting documents
requirements.txt
Lists all required Python libraries
README.md
Project description and usage instructions
---
## How to Run the Project
1. Open the notebook in Google Colab
2. Mount Google Drive
3. Load the dataset
4. Run all cells in the notebook
5. Train and evaluate the model
---
## Applications
This project demonstrates how Machine Learning can be used for:
* Medical image classification
* Disease detection using AI
* Automated diagnostic systems
* Healthcare decision support systems
---
## Author
**Muhammad Abdullah Awan**
BS Artificial Intelligence
COMSATS University Islamabad – Wah Campus
