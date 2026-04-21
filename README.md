<div align="center">

# Drowsiness Detection Using Computer Vision & Deep Learning

[![Python](https://img.shields.io/badge/Python-3.11-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![OpenCV](https://img.shields.io/badge/OpenCV-Computer_Vision-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white)](https://opencv.org)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-CNN-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)](https://tensorflow.org)
[![Domain](https://img.shields.io/badge/Domain-Safety_AI-ef4444?style=for-the-badge)](.)

> Real-time driver drowsiness and yawn detection - triggers an audio alert the moment fatigue is detected.

</div>

---

## Why This Matters

Driver fatigue causes **20% of road accidents** worldwide. This system monitors a driver in real time and sounds an alert the moment drowsiness is detected.

---

## How It Works

```
Webcam Feed
     |
     v
Face Detection (OpenCV + Haar Cascade)
     |
     v
Eye Region Crop --> CNN Classifier --> Open / Closed
     |
     v
Drowsiness Logic
  - Eyes closed beyond threshold --> AUDIO ALERT
  - Yawn detected (Mouth Aspect Ratio) --> AUDIO ALERT
```

---

## Detection Capabilities

| Feature | Method |
|---|---|
| **Eye State** | CNN trained on eye open/close dataset |
| **Yawn Detection** | Mouth Aspect Ratio (MAR) threshold |
| **Face Localisation** | OpenCV Haar Cascade / dlib 68-point landmarks |
| **Alert System** | Real-time audio warning on fatigue detection |

---

## Performance

| Metric | Result |
|---|---|
| Accuracy | ~96% on test set |
| Inference | Real-time at 30 FPS |
| False Positive Rate | < 5% |

---

## Tech Stack

```
OpenCV       - real-time video capture and face detection
TensorFlow   - CNN eye state classification model
dlib         - 68-point facial landmark detection
pygame       - audio alert playback
numpy        - frame array processing
```

---

## Run Locally

```bash
git clone https://github.com/arunima-anil/Drowsiness-Detection-Using-Computer-Vision-and-Deep-Learning
cd Drowsiness-Detection-Using-Computer-Vision-and-Deep-Learning
pip install -r requirements.txt
python detect.py
```

> Requires a webcam. Press Q to quit.

---

<div align="center">Built as part of AI & Data Science portfolio | <a href="https://github.com/arunima-anil">@arunima-anil</a></div>
