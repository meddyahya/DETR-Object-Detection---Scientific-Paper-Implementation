# Tiny-DETR Object Detection - Scientific Paper Implementation

Compact implementation of **DETR (Detection Transformer)** for object detection, focused on **pedestrian detection** using the PennFudanPed dataset. This project explores transformer depth, backbone choices, query counts, and data augmentation techniques in a small-dataset regime, achieving approximately 0.51 mAP@0.5 with an end-to-end Hungarian matching-based detector.

Original Paper: https://arxiv.org/abs/2005.12872

## Outline

- [About](#about)
- [Background](#background)
- [Features](#features)
- [Dataset](#dataset)
- [Results](#results)
- [Installtion](#installation)

## About

This repository implements a **compact variant of DETR** originally proposed in the paper *End-to-End Object Detection with Transformers* by Nicolas Carion et al. DETR formulates object detection as a direct set prediction problem using a transformer encoder–decoder architecture, simplifying the detection pipeline by removing NMS and anchors.

## Background
Traditional object detectors rely on many hand-designed components (e.g., anchors, NMS). DETR instead uses a transformer to directly predict object bounding boxes and class labels in parallel, with a bipartite matching loss that enforces unique predictions per object.

## Features
- Compact DETR implementation in PyTorch  
- End-to-end transformer-based object detection  
- Hungarian matching loss  
- Customizable transformer depth and backbone  
- Pedestrian detection on PennFudanPed dataset

## Dataset
This project uses the **PennFudanPed dataset**:
- Pedestrian images with segmentation masks and bounding boxes
- Organized into training/validation splits

## Results
<img width="4500" height="1500" alt="best_model_predicted" src="https://github.com/user-attachments/assets/ba15716a-0138-47ef-b4b1-8371b36b07c9" />


## Installation

Clone the repo:
```bash
git clone https://github.com/meddyahya/DETR-Object-Detection---Scientific-Paper-Implementation.git
cd DETR-Object-Detection---Scientific-Paper-Implementation
```

Install the dependencies:
```bash
pip install -r requirements.txt
```

