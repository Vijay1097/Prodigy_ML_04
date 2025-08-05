# ✋ Hand Gesture Recognition System with Real Image Data + Fallback Generator

This project implements a *Hand Gesture Recognition System* using real images collected online and synthetically generated landmark patterns. The model supports gestures: *1, 2, 3, 4, 5, and hi*.

> 🔍 Inspired by real-world applications of gesture-controlled navigation and interaction systems.

---

## 🚀 Features

- 🖐 Recognizes gestures: 1, 2, 3, 4, 5, and hi
- 🌐 Downloads real images from *Unsplash* and *Pixabay*
- 🎨 Generates synthetic fallback hand landmarks
- 🔍 Uses *MediaPipe* to extract hand landmarks from images
- 🤖 Trains a *Random Forest Classifier* for gesture recognition
- 📈 Includes accuracy report and confusion matrix
- 🧪 Offers both *image upload* and *dataset test modes*
- 🔗 Built for Google Colab compatibility

---

## 🧠 Technologies Used

| Tool/Library        | Purpose                     |
|---------------------|-----------------------------|
| mediapipe         | Hand landmark extraction    |
| opencv-python     | Image handling and display  |
| scikit-learn      | Random Forest, Evaluation   |
| matplotlib/seaborn| Visualization               |
| beautifulsoup4    | Web scraping image URLs     |
| Pillow            | Image processing            |
| Google Colab      | Execution environment       |

---

## 🛠 Installation

bash
pip install mediapipe opencv-python scikit-learn numpy matplotlib requests pillow beautifulsoup4 seaborn


---

## 📁 Directory Structure


├── recognizer.py                    # Core implementation
├── gesture 1 output.jpg             # Sample output for gesture "1"
├── gesture Hi output.jpg            # Sample output for gesture "hi"
└── README.md


---

## 📸 Sample Output (Visual)

### ➕ Gesture: 1

![Gesture 1](https://github.com/Vijay1097/Prodigy_ML_04/blob/main/gesture%201%20output.jpg)

*Prediction*: 1  
*Confidence*: ~96.3%

---

### 👋 Gesture: hi

![Gesture Hi](https://github.com/Vijay1097/Prodigy_ML_04/blob/main/gesture%20Hi%20output.jpg)

*Prediction*: hi  
*Confidence*: ~91.5%

---

## 🧪 Testing Options

- test_single_image() → Upload your own hand gesture image  
- test_training_images() → Run evaluation on training/test data  
  - Mode 1: Random test  
  - Mode 2: Choose specific gesture  
  - Mode 3: Test all gestures  
  - Mode 4: Interactive browse

---

## 📊 Model Performance

| Metric            | Value     |
|-------------------|-----------|
| Training Accuracy | ~92%      |
| Testing Accuracy  | ~87%      |

Confusion Matrix and Classification Report are plotted and printed post-training.

---

## 🔍 How it Works

1. *Image Collection*: Downloads real hand gesture images from multiple online sources using keyword search.
2. *Landmark Extraction*: MediaPipe extracts 21 hand landmark positions (x, y, z).
3. *Fallback Data*: If real images are missing, synthetic patterns fill the gap using finger-tip templates.
4. *Model Training*: Random Forest trained with noise-injected data to simulate realistic performance.
5. *Prediction*: For any input image, landmarks are extracted and classified into one of six gestures.

---

## 🧑‍💻 Author

*Comillas Negras – Task 05*  
Food & Gesture Recognition AI Challenge

---

## ✅ Future Work

- ✨ Extend to dynamic gestures or video input  
- 📦 Deploy as a Web or Mobile App  
- 🔤 Multi-language gesture classification  
- 🥗 Integrate with calorie tracking for food-hand gestures

---

## 📬 Contact

Feel free to open issues or contribute via pull requests.
