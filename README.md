# 🌱 AI-Powered Greenhouse Insect Detection

### Deep Learning-Based Detection and Classification of Insects on Yellow Sticky Traps

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![YOLOv8](https://img.shields.io/badge/YOLOv8-Object%20Detection-orange)
![RF-DETR](https://img.shields.io/badge/RF--DETR-Object%20Detection-purple)
![Computer Vision](https://img.shields.io/badge/Computer%20Vision-Deep%20Learning-green)

> An AI-based computer vision research project for automatic detection and classification of harmful and beneficial insects in greenhouse yellow sticky trap images.

**YOLOv8 • RF-DETR • Deep Learning • Computer Vision • Object Detection • Precision Agriculture**

---

## 🚀 Project Overview

Manual counting of insects on yellow sticky traps is time-consuming and difficult to use for continuous monitoring.

This project investigates deep learning-based methods for automatically detecting and classifying insects captured in greenhouse environments.

The research focuses on three insect species:

| Class | Species | Category |
|---|---|---|
| **WF** | *Trialeurodes vaporariorum* | Harmful insect |
| **MR** | *Macrolophus pygmaeus* | Beneficial insect |
| **NC** | *Nesidiocoris tenuis* | Beneficial insect |

The object detection stage uses **YOLOv8** and **RF-DETR**. Detected insects are subsequently classified using deep learning models including **VGG19, ResNet50, NASNet Mobile and FGCN**.

---

## 🎯 Research Pipeline

```text
Greenhouse Images
       │
       ▼
Image Preprocessing
       │
       ▼
Manual Annotation
       │
       ▼
YOLOv8 / RF-DETR
Object Detection
       │
       ▼
Detected Insects
       │
       ▼
Deep Learning Classification
       │
       ▼
Insect Species
🧠 Object Detection

Two object detection models were investigated:

YOLOv8

YOLOv8 was evaluated for detecting insects appearing on yellow sticky trap images.

RF-DETR

RF-DETR was investigated as a transformer-based object detection approach and compared with YOLOv8.

📊 YOLOv8 Results

The YOLOv8 model achieved the following results:

Metric	Result
Precision	85.6%
Recall	77.9%
mAP@50	81.6%
mAP@50–95	41.3%
Class-Level Performance
Class	Precision	Recall	mAP@50	mAP@50–95
MR	89.2%	74.8%	82.6%	39.8%
NC	80.4%	79.7%	76.1%	45.7%
WF	87.3%	79.1%	86.1%	38.4%
🔬 Training Configuration
Parameter	Value
Model	YOLOv8n
Epochs	20
Batch Size	10
Image Size	1024 × 1024
Optimizer	SGD
Learning Rate	0.0001
GPU	NVIDIA RTX 3080
Augmentation	HSV, Mosaic, MixUp, Horizontal Flip
📈 Training & Evaluation

The training and evaluation process includes:

Training curves
mAP curves
Confusion matrix
Class-level metrics
Detection examples
YOLOv8 vs RF-DETR comparison

The corresponding visualizations will be added to the results/ directory.

🗂️ Dataset

The research dataset contains images collected from greenhouse environments using Scoutbox and smartphone-based image acquisition.

The dataset includes:

225 selected Scoutbox images
90 smartphone images
Image patches generated from the collected images
Expert/manual annotations
Three insect classes

The object detection annotations contain:

WF → 5611 annotations
MR → 1314 annotations
NC →  511 annotations

Manual annotation was performed using LabelImg.

Dataset DOI:
10.4121/uuid:8b8ba63a-1010-4de7-a7fb-6f9e3baf128e

The original dataset is not redistributed in this repository.

🔄 YOLOv8 vs RF-DETR

The research compared the two object detection approaches:

Model	mAP@50	mAP@50–95
YOLOv8	81.6%	41.3%
RF-DETR	77.1%	35.8%
🖼️ Detection Examples

Detection visualizations will show:

Original yellow sticky trap images
Bounding boxes
Detected insect classes
Confidence scores
Multiple insects in the same image

Detection result images will be added to this section.

🧪 Classification

Following object detection, the detected insects were classified using several deep learning architectures.

Models investigated include:

VGG19
ResNet50
NASNet Mobile
FGCN

The VGG19 model achieved 97.05% accuracy, while NASNet Mobile achieved 91.53% accuracy. FGCN achieved 59.98% accuracy.

🛠️ Technologies
Python
YOLOv8
RF-DETR
Deep Learning
Computer Vision
Object Detection
Image Classification
LabelImg
COCO Annotation Format
GPU-Accelerated Training
📁 Repository Structure
greenhouse-insect-detection/
│
├── README.md
│
├── app/
│   └── app.py
│
├── src/
│   ├── detector.py
│   ├── inference.py
│   └── visualization.py
│
├── models/
│   └── README.md
│
├── demo/
│   ├── images/
│   └── videos/
│
├── results/
│   ├── training_curves.png
│   ├── confusion_matrix.png
│   ├── class_metrics.png
│   ├── model_comparison.png
│   └── detection_examples.png
│
├── notebooks/
│   └── inference_demo.ipynb
│
└── docs/
    ├── dataset.md
    ├── methodology.md
    └── results.md
📄 Published Research
YOLOv8 ve RF-DETR Kullanılarak Sarı Yapışkan Tuzaklardaki Böceklerin Yapay Zeka Destekli Tespiti ve Sınıflandırılması: Hassas Tarım için Derin Öğrenme Yaklaşımı

Authors: Fatma Öncü, Fehim Köylü

This research was developed as part of my master's thesis and investigates deep learning-based insect detection and classification in greenhouse environments.

DOI: 10.65520/erciyesfen.1748404

Published Article:
https://dergipark.org.tr/tr/pub/erciyesfen/article/1748404

🎓 Master's Thesis

Title:
DETECTION OF PESTS IN GREENHOUSES USING DEEP LEARNING TECHNIQUES

Author: Fatma ÖNCÜ

Institution: Erciyes University, Graduate School of Natural and Applied Sciences

Degree: Master Thesis

Year: 2025

👩‍💻 Author
Fatma Öncü

Computer Engineer | Deep Learning & Computer Vision

GitHub:
https://github.com/fatma-oncu

📌 Project Status

🚧 Research & Portfolio Project

 YOLOv8 object detection
 RF-DETR object detection
 Experimental evaluation
 Classification experiments
 Published research
 Interactive demo
 Inference application
 Final visualization gallery
 Complete repository documentation
⭐ Research Focus

Computer Vision + Deep Learning + Object Detection + Insect Recognition + Precision Agriculture

This project explores AI-assisted approaches for automated insect monitoring in greenhouse environments
