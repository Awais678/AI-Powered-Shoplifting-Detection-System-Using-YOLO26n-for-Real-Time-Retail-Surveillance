# 🛒 AI-Powered-Shoplifting-Detection-System-Using-YOLO26n-for-Real-Time-Retail-Surveillance

A real-time **Shoplifting Detection System** developed using a custom **YOLO26n** object detection model. The system detects suspicious shoplifting behavior from surveillance camera feeds by identifying two classes: **Shoplifting** and **Not Shoplifting**. It supports image, video, and live webcam inference, making it suitable for intelligent retail security and automated surveillance.

---

## 🚀 Features

- Real-time shoplifting behavior detection
- Supports image, video, and live webcam inference
- Detects suspicious activities with confidence scores
- Displays bounding boxes and status labels
- Lightweight YOLO26n model for fast inference
- Suitable for CCTV-based surveillance systems

---

## 📊 Detection Classes

The model classifies human activities into:

- 🟥 Shoplifting
- 🟩 Not Shoplifting

---

## 🛠️ Technologies Used

- Python
- YOLO26n (Ultralytics)
- OpenCV
- NumPy
- Google Colab

---

## 📁 Dataset Structure

```
dataset/
├── train/
│   ├── images/
│   └── labels/
├── valid/
│   ├── images/
│   └── labels/
├── test/
│   ├── images/
│   └── labels/
└── data.yaml
```

---

## 📈 Model Performance

The custom YOLO26n model was trained on a labeled shoplifting dataset for binary activity detection.

| Metric | Value |
|---------|------:|
| **mAP@50** | **XX.X%** |
| **mAP@50-95** | **XX.X%** |
| **Precision** | **XX.X%** |
| **Recall** | **XX.X%** |
| **F1-Score** | **XX.X%** |

> Replace the values above with your actual training results from `results.csv` or `results.png`.

---

## ⚙️ Training Details

| Parameter | Value |
|-----------|-------|
| Model | YOLO26n |
| Image Size | 640 × 640 |
| Epochs | 100 |
| Batch Size | 16 |
| Framework | Ultralytics YOLO |
| Classes | Shoplifting, Not Shoplifting |

---

## ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/shoplifting-detection-yolo.git
cd shoplifting-detection-yolo
```

Install dependencies:

```bash
pip install -r requirements.txt
```

or

```bash
pip install ultralytics opencv-python numpy
```

---

## 🏋️ Model Training

```python
from ultralytics import YOLO

model = YOLO("yolo26n.pt")

model.train(
    data="data.yaml",
    epochs=100,
    imgsz=640,
    batch=16
)
```

---

## 🖼️ Image Inference

```python
from ultralytics import YOLO

model = YOLO("best.pt")

results = model("image.jpg", save=True)
```

---

## 🎥 Video Inference

```python
from ultralytics import YOLO

model = YOLO("best.pt")

model.predict(
    source="video.mp4",
    save=True
)
```

---

## 📷 Webcam Inference

```python
from ultralytics import YOLO

model = YOLO("best.pt")

model.predict(
    source=0,
    show=True
)
```

---

## 📂 Project Structure

```
Shoplifting-Detection-using-YOLO/
│
├── dataset/
├── runs/
│   └── detect/
│       └── train/
│           └── weights/
│               ├── best.pt
│               └── last.pt
│
├── shoplifting_detection_using_YOLO.ipynb
├── inference.py
├── train.py
├── data.yaml
├── requirements.txt
├── README.md
└── LICENSE
```

---

## 📈 Output

For each detected person, the model provides:

- Activity label
- Confidence score
- Bounding box
- Real-time status visualization

Example:

```
Shoplifting       94%
Not Shoplifting   97%
```

---

## 💡 Applications

- Smart Retail Security
- CCTV Surveillance
- Theft Prevention
- Automated Shop Monitoring
- Loss Prevention Systems
- AI-powered Security Analytics
- Retail Store Automation

---

## 🔮 Future Improvements

- Integrate multi-object tracking (ByteTrack/DeepSORT)
- Reduce false positives using temporal action analysis
- Deploy on edge devices (Jetson Nano, Raspberry Pi)
- Web dashboard for real-time monitoring
- Automatic alert system via SMS or Email
- Cloud-based surveillance analytics

---

## 📜 License

This project is licensed under the **MIT License**.

---

## 👨‍💻 Author

**Awais Ahmed**

Electrical Engineering, NUST Islamabad

**Interests:** Computer Vision, Deep Learning, Artificial Intelligence, Embedded Systems, Intelligent Surveillance

---

## ⭐ Support

If you found this project helpful, please give this repository a **⭐ Star** on GitHub.

Contributions, suggestions, and pull requests are always welcome!
