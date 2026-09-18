# 🌱 AI-Powered Greenhouse Insect Detection

### Deep Learning-Based Detection and Classification of Insects on Yellow Sticky Traps

[![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)]
[![YOLOv8](https://img.shields.io/badge/YOLOv8-Object%20Detection-orange)]
[![RF-DETR](https://img.shields.io/badge/RF--DETR-Object%20Detection-purple)]
[![Computer Vision](https://img.shields.io/badge/Computer%20Vision-Deep%20Learning-green)]

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

The object detection stage uses **YOLOv8** and **RF-DETR**. Detected insects are subsequently classified using deep learning models including VGG19, ResNet50, NASNet Mobile and FGCN. :contentReference[oaicite:1]{index=1}

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
