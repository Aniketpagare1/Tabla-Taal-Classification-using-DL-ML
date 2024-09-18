
# 🎶 Tabla Taal Classification using Deep Learning and Machine Learning


This project uses **deep learning** and **machine learning** techniques to classify different **taals (rhythmic patterns)** of the Indian classical percussion instrument, **Tabla**. The goal is to accurately predict and classify the taal based on input audio files.

The system is designed to take in an audio file (wav format), preprocess it, and use a trained **deep learning model** to classify it into a specific **taal**.

---

## 🛠️ Features

- **Audio Processing**: Preprocessing of audio files to extract features using **MFCC** (Mel Frequency Cepstral Coefficients).
- **Taal Classification**: Classifies the input tabla audio into various taals using a trained model.
- **Pre-trained Model**: Utilizes a pre-trained **deep learning model** for accurate classification.
- **Flask Web App**: Provides a web interface for users to upload audio files and get the predicted taal.

---

## 📂 Project Structure

```txt
tabla-taal-classification-using-dl-ml/
│
├── Model.py                # Model training script
├── app.py                  # Flask web application
├── data.csv                # CSV file containing training data
├── encoder.pkl             # Label encoder for categorical conversion
├── model.pkl               # Pre-trained classification model
├── scaler.pkl              # Scaler used to normalize input features
├── test.py                 # Test script for local predictions
├── xyz.wav                 # Sample audio file
├── README.md               # Instructions (this file)

```

---

## 🚀 Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/Aniketpagare1/Tabla-Taal-Classification-using-DL-ML.git
cd Tabla-Taal-Classification-using-DL-ML
```

### 2. Install Dependencies

Install the required Python dependencies by running:



## 🛠️ Usage

### 1. Run Flask Web App

To use the web interface, run the Flask app using:

```bash
python app.py
```

1. **Open Web Browser**: Navigate to `http://127.0.0.1:5000/` in your web browser.
2. **Upload Audio File**: Upload an audio file (wav format) and get the predicted **taal**.

### 2. Local Testing

You can also test the model locally by running the `test.py` script:

```bash
python test.py
```

- This script loads the pre-trained model and performs classification on the provided audio file (such as `xyz.wav`).

---

## 🧠 Model Training

If you want to train the model yourself, you can use the `Model.py` script to retrain the deep learning model.

1. **Prepare Data**: The `data.csv` file contains the dataset for training. Ensure that the data is properly formatted with audio features and labels.
2. **Train Model**: Run `Model.py` to train the model:

```bash
python Model.py
```

The script will generate a new model and save it as `model.pkl`.

---

## 📈 Model Evaluation

The model is evaluated using standard metrics such as **accuracy**, **precision**, and **recall**. After training, the evaluation results will be displayed on the console.

---

## 🔑 Techniques Used

- **MFCC (Mel Frequency Cepstral Coefficients)**: Extract features from audio data.
- **Deep Learning**: Neural networks are used to classify taals based on extracted features.
- **Label Encoding**: The categorical labels (taals) are encoded using `encoder.pkl`.
- **Feature Scaling**: Input features are scaled using `scaler.pkl` to ensure proper training.

---

## 📂 Example Input

Example of a **wav** file (like `xyz.wav`) is provided to test the model.

---

## 🧪 Example

```txt
Input: xyz.wav
Predicted Taal: "Teentaal"
```

---

## 📜 License

This project is open source and available under the **MIT License**.

---
