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

## 📊 Model Performance

The custom **YOLO26n** model was trained for **60 epochs** on a labeled shoplifting detection dataset and achieved strong performance for real-time retail surveillance.

### Overall Performance

| Metric | Value |
|---------|------:|
| **Precision** | **70.3%** |
| **Recall** | **86.5%** |
| **mAP@50** | **84.3%** |
| **mAP@50-95** | **62.4%** |

### Class-wise Performance

| Class | Precision | Recall | mAP@50 | mAP@50-95 |
|-------|----------:|-------:|--------:|----------:|
| **Normal** | 70.9% | 85.1% | 83.3% | 58.3% |
| **Shoplifting** | 69.7% | 88.0% | 85.3% | 66.5% |

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

## 💡 Applications

- Smart Retail Security
- CCTV Surveillance
- Theft Prevention
- Automated Shop Monitoring
- Loss Prevention Systems
- AI-powered Security Analytics
- Retail Store Automation

---

## 📈 Key Highlights

- ✅ Achieved **84.3% mAP@50** on the validation dataset.
- ✅ Obtained **86.5% recall**, enabling reliable detection of shoplifting incidents.
- ✅ Lightweight **5.4 MB YOLO26n** model suitable for real-time deployment.
- ✅ Successfully distinguishes between **Normal** and **Shoplifting** activities from CCTV footage.
- ✅ Optimized for fast inference while maintaining high detection accuracy.
