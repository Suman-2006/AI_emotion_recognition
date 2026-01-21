🧠 AI Facial Emotion Recognition System

A real-time Facial Emotion Recognition system built using Deep Learning (CNN), TensorFlow, and OpenCV.
The model is trained on the FER dataset and can detect human emotions from a webcam feed, logging predictions to a CSV file for analysis.

🚀 Features

🎭 Detects 7 human emotions:

Angry

Disgusted

Fearful

Happy

Neutral

Sad

Surprised

📷 Real-time emotion recognition using webcam

🧠 Custom CNN trained from scratch

🧾 Logs predictions with timestamp & confidence to CSV

🟩 Face detection using Haar Cascade

🧪 End-to-end ML pipeline (training → inference)

🗂️ Project Structure
AI-Face-Emotion-Recognition/
│
├── emotion_recognition.py      
├── train_emotion_model.py        
├── haarcascade_frontalface_default.xml
├── requirements.txt
├── .gitignore
│
├── models/
│   └── emotion_model.h5          
│
├── dataset/                     
├── emotion_log.csv              
└── venv/                    

🧠 Model Details

Architecture: Convolutional Neural Network (CNN)

Input Shape: (48, 48, 1) (grayscale)

Output Classes: 7 emotions

Optimizer: Adam

Loss Function: Sparse Categorical Crossentropy

Training Accuracy: ~62% (CPU training)

⚙️ Installation & Setup
1️⃣ Clone the Repository
git clone https://github.com/Suman-2006/AI_emotion_recognition.git
cd AI-Face-Emotion-Recognition

2️⃣ Create Virtual Environment
python -m venv venv


Activate:

Windows

venv\Scripts\activate

3️⃣ Install Dependencies
pip install -r requirements.txt

🏋️‍♂️ Training the Model

Make sure the FER dataset is placed inside dataset/train/

python train_emotion_model.py


This will:

Train the CNN

Save the model to models/emotion_model.h5

🎥 Run Real-Time Emotion Detection
python emotion_recognition.py

Controls:

Press Q or ESC to quit

Ensure the camera window is focused

🧾 CSV Logging

All predictions are saved automatically to:

emotion_log.csv


Format:

timestamp,emotion,confidence
2026-01-21 12:10:34,happy,0.82


This allows:

Emotion trend analysis

Visualization

Dataset creation

🧪 Technologies Used

Python

TensorFlow / Keras

OpenCV

NumPy

Haar Cascade Classifier

Git & GitHub

📌 Use Cases

Human–Computer Interaction

Emotion analytics

Mental health research

Smart surveillance systems

AI-based user experience analysis

🏆 What I Learned

Building CNNs from scratch

Image preprocessing & normalization

Matching training and inference pipelines

Real-time computer vision

Debugging ML + system-level issues

Professional GitHub workflow

🔮 Future Improvements

Add validation & test accuracy

Data augmentation for better accuracy

Flask API for web integration

MERN frontend integration

Emotion analytics dashboard

👤 Author

Suman Raju Kojalagi


⭐ If you like this project

Give it a ⭐ on GitHub and feel free to fork or contribute!