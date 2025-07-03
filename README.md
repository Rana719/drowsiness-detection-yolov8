# 🛑 Drowsiness Detection Using YOLOv8

This project uses **YOLOv8** and **Computer Vision** to detect signs of driver drowsiness and inattention in real-time video streams. It classifies 9 distinct states such as "eyes closed", "head down", "yawning", and more using a custom-trained deep learning model.

---

## 🎯 Project Goal

> Detect if a driver is drowsy using AI in real-time video.

---

## 🧠 Model Summary

- **Model**: YOLOv8n (nano version)
- **Framework**: Ultralytics YOLOv8
- **Training Platform**: Google Colab (for GPU acceleration)
- **Evaluation Metrics**:
  - **Precision**: 0.974
  - **Recall**: 0.978
  - **mAP@0.5**: 0.991
  - **mAP@0.5:0.95**: 0.958

---

## 🧾 Classes Detected (9 total)

| Class Name                | Instances | mAP@0.5 |
|--------------------------|-----------|---------|
| `eyes_closed`            | 80        | 0.989   |
| `eyes_closed_head_left`  | 40        | 0.980   |
| `eyes_closed_head_right` | 37        | 0.993   |
| `focused`                | 65        | 0.995   |
| `head_down`              | 67        | 0.988   |
| `head_up`                | 78        | 0.995   |
| `seeing_left`            | 55        | 0.992   |
| `seeing_right`           | 46        | 0.991   |
| `yarning`                | 62        | 0.995   |

---

## 🛠️ Tech Stack

- [YOLOv8](https://github.com/ultralytics/ultralytics)
- Python
- OpenCV
- Jupyter Notebook
- Google Colab (for training)

---

## 📂 Dataset

- **Total Images**: 6391
- **Split**:
  - Training Set: 5595 images (88%)
  - Validation Set: 530 images (8%)
  - Test Set: 266 images (4%)
- **Source**: [Roboflow Public Dataset](https://universe.roboflow.com/karthik-madhvan/drowsiness-detection-xsriz/dataset/1)
- **Format**: YOLOv8-ready with `data.yaml`

---

## 🏁 How to Run the Project

### 📦 1. Clone the repository

```bash
git clone https://github.com/Rana719/drowsiness-detection-yolov8.git
cd drowsiness-detection-yolov8
