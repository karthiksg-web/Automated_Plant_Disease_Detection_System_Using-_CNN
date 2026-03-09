# 🌿 Automated Plant Disease Detection System Using CNN

A deep learning-based system for detecting and classifying plant diseases from leaf images using Convolutional Neural Networks (CNN) built with TensorFlow/Keras.

---

## 📌 Overview

This project uses a CNN model trained on the **PlantVillage dataset** to detect diseases across multiple plant species. The model is deployed as a web application built with **Streamlit**, allowing users to upload a leaf image and get an instant disease diagnosis.

---

## 🚀 Features

- ✅ Detects **38 disease classes** across multiple plant species
- ✅ Trained CNN model with high accuracy
- ✅ Simple web interface powered by **Streamlit**
- ✅ Real-time prediction with confidence score
- ✅ Supports common image formats (JPG, PNG)

---

## 📁 Project Structure

```
├── main.py                      # Streamlit web app
├── Train_plant_disease.ipynb    # Model training notebook
├── Test_plant_disease.ipynb     # Model testing/evaluation notebook
├── trained_model.keras          # Pre-trained CNN model (via Git LFS)
├── training_hist.json           # Training history (accuracy & loss)
├── home_page.jpeg               # Home page image for the app
├── requirement.txt              # Python dependencies
└── README.md
```

---

## 📦 Dataset

The model is trained on the **New Plant Diseases Dataset** available on Kaggle:

> 🔗 **[New Plant Diseases Dataset – Kaggle](https://www.kaggle.com/datasets/vipoooool/new-plant-diseases-dataset)**

The dataset contains **87,000+ RGB images** of healthy and diseased crop leaves categorized into **38 classes**, split into:
- `train/` – Training images
- `valid/` – Validation images
- `test/` – Test images

---

## 🛠️ Installation & Setup

### 1. Clone the Repository
```bash
git clone https://github.com/karthiksg-web/Automated_Plant_Disease_Detection_System_Using-_CNN.git
cd Automated_Plant_Disease_Detection_System_Using-_CNN
```

### 2. Install Dependencies
```bash
pip install -r requirement.txt
```

### 3. Download the Dataset
Download the dataset from Kaggle:
👉 [https://www.kaggle.com/datasets/vipoooool/new-plant-diseases-dataset](https://www.kaggle.com/datasets/vipoooool/new-plant-diseases-dataset)

Place the extracted folders (`train/`, `valid/`, `test/`) inside the project directory.

### 4. Run the App
```bash
streamlit run main.py
```

---

## 🧠 Model Architecture

The CNN model was built using **TensorFlow/Keras** and trained on the PlantVillage dataset:

- Multiple **Conv2D + MaxPooling** layers for feature extraction
- **Dropout** layers to prevent overfitting
- **Dense** layers for classification
- Output: **38 classes** (softmax activation)

---

## 📊 Training Results

Training history (accuracy and loss per epoch) is saved in `training_hist.json`. Open the `Train_plant_disease.ipynb` notebook to view training curves.

---

## 🌱 Supported Plants & Diseases

The model can detect diseases in:
Apple, Blueberry, Cherry, Corn, Grape, Orange, Peach, Pepper, Potato, Raspberry, Soybean, Squash, Strawberry, Tomato and more.

---

## 📋 Requirements

See `requirement.txt` for full list. Main dependencies:
- TensorFlow / Keras
- Streamlit
- NumPy
- Pillow (PIL)
- Matplotlib

---

## 📄 License

This project is for educational purposes. The dataset is provided by [vipoooool on Kaggle](https://www.kaggle.com/datasets/vipoooool/new-plant-diseases-dataset).

---

## 🙌 Acknowledgements

- Dataset: [New Plant Diseases Dataset](https://www.kaggle.com/datasets/vipoooool/new-plant-diseases-dataset) by vipoooool on Kaggle
- Framework: TensorFlow / Keras
- App: Streamlit
