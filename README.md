# Garbage-Classification-w-YOLOv8

This project focuses on detecting and classifying garbage using a custom-trained YOLOv8 object detection model. The goal is to enable intelligent waste recognition to support smart environmental monitoring, recycling systems, or cleanliness auditing.

The model is trained on a dataset obtained from Roboflow and evaluated using standard metrics like mAP, precision, and recall. Example predictions and confidence scores are included in the notebook for inspection.

---

## 📌 Overview

This project aims to automate garbage classification using computer vision. It includes:

- Dataset download from Roboflow (YOLO format)
- Training with YOLOv8s
- Saving & reloading trained model
- Inference with bounding boxes and confidence scores
- Model evaluation using standard detection metrics

---

## 🗂️ Classes Detected

- `BIODEGRADABLE`
- `CARDBOARD`
- `GLASS`
- `METAL`
- `PAPER`
- `PLASTIC`

---

## 🧪 Model Evaluation (Validation Set)

| Class         | Precision | Recall | mAP@0.5 | mAP@0.5:0.95 |
|---------------|-----------|--------|---------|--------------|
| BIODEGRADABLE | 0.815     | 0.492  | 0.638   | 0.366        |
| CARDBOARD     | 0.747     | 0.538  | 0.638   | 0.482        |
| GLASS         | 0.884     | 0.705  | 0.819   | 0.619        |
| METAL         | 0.792     | 0.623  | 0.720   | 0.495        |
| PAPER         | 0.039     | 0.060  | 0.077   | 0.070        |
| PLASTIC       | 0.446     | 0.537  | 0.462   | 0.302        |
| **Overall**   | **0.620** | **0.493** | **0.559** | **0.389**  |

> 📍 Trained with `yolov8s.pt`, 50 epochs, image size 640×640, batch size 32  
> 💾 Evaluation performed on 2,098 validation images using 18,916 instances.

---

## 🖼️ Sample Inference

The notebook includes prediction on test images with class names and confidence levels printed:

<img width="520" height="515" alt="image" src="https://github.com/user-attachments/assets/46a7f7f2-8c98-413c-b186-f0445f1ec723" />
