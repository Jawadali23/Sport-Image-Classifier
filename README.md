# 🏆 Sport Image Classifier

A machine learning project that classifies sports personalities using computer vision and image processing techniques. The model detects faces, extracts key features, and predicts the corresponding sports category.

---

## 📌 Project Overview

This project focuses on building an image classification system using:

* **OpenCV** for image processing and face/eye detection
* **Machine Learning models** for classification
* **Feature engineering techniques** like grayscale conversion and region extraction

The system ensures better accuracy by only using images where **at least two eyes are detected**, improving data quality.

---

## 🚀 Features

* ✅ Face detection using Haar Cascades
* ✅ Eye detection for validation
* ✅ Automatic image cropping
* ✅ Clean dataset generation
* ✅ Trained classification model (`saved_model.pkl`)
* ✅ Visualization using Matplotlib

---

## 🧠 Workflow

1. **Load Image**
2. **Convert to Grayscale**
3. **Detect Face**
4. **Detect Eyes**
5. **Filter Images (only keep images with 2+ eyes)**
6. **Crop Face Region**
7. **Train ML Model**
8. **Save Model**

---

## 🗂️ Project Structure

```
Sport-Image-Classifier/
│
├── images_dataset/              # Raw dataset
├── cropped_images/             # Processed dataset
├── Opencv/
│   ├── haarcascade_frontalface_default.xml
│   └── haarcascade_eye.xml
│
├── Test_data/                  # Sample test images
├── saved_model.pkl             # Trained model
├── SportImageClassifier.ipynb  # Main notebook
└── README.md
```

## 📊 Example

* Input: Image of a sports personality
* Output: Predicted class (e.g., Tennis Player, Cricketer, etc.)

---

## 📈 Technologies Used

* Python
* OpenCV
* NumPy
* Matplotlib
* Scikit-learn

---

## 🔍 Key Function

```python
def get_cropped_image_if_2_eyes(image_path):
```

This function:

* Detects face
* Checks for at least 2 eyes
* Returns cropped face image

---

## 💡 Future Improvements

* 🔹 Use Deep Learning (CNN) for higher accuracy
* 🔹 Deploy as a Web App
* 🔹 Add real-time webcam prediction
* 🔹 Improve dataset diversity

