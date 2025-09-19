🚀 Overview
Early detection of skin cancer is critical for improving patient outcomes, but manual diagnosis can be time-consuming and subjective. This project addresses this challenge by developing an automated classification system using efficient Convolutional Neural Networks (CNNs). By leveraging transfer learning with lightweight models, this solution is designed for high accuracy and is suitable for deployment on resource-constrained devices, such as mobile phones.

✨ Features
Multi-Class Classification: Classifies dermoscopic images into seven distinct lesion categories (e.g., Melanoma, Basal cell carcinoma).

Efficient Architectures: Implements and compares two modern, efficient models: MobileNetV2 and MobileNetV3.

Transfer Learning: Utilizes models pre-trained on ImageNet and fine-tunes them for the specific task of skin lesion classification.

Robust Preprocessing: Includes denoising, resizing, and normalization to standardize images for the model.

Data Augmentation: Employs random flips and rotations to create a more robust training set and prevent overfitting.

Class Imbalance Handling: Explores class-weighted training with MobileNetV3 to improve performance on under-represented classes.

🛠️ Technology Stack
Models: MobileNetV2, MobileNetV3

Framework: PyTorch

Core Libraries: Python, OpenCV, Pandas, Scikit-learn, Matplotlib

⚙️ Setup & Installation
To run this project, you would typically follow these steps:

Clone the repository (replace YOUR_USERNAME with your actual GitHub username):

git clone [https://github.com/YOUR_USERNAME/skin-cancer-classification.git](https://github.com/YOUR_USERNAME/skin-cancer-classification.git)
cd skin-cancer-classification

Install dependencies from a requirements.txt file:

pip install -r requirements.txt

Run the Jupyter Notebook or training script.

📈 Model Performance
Two models were trained and evaluated for 50 epochs.

1. MobileNetV2
This model achieved the highest overall accuracy.

Validation Accuracy: 79.90%

Validation Loss: 0.6287

2. MobileNetV3 (with Class-Weighted Loss)
This model was designed to be more robust against the imbalanced dataset, showing better-balanced performance across all classes.

Validation Accuracy: 73.90%

Validation Loss: 0.7722
