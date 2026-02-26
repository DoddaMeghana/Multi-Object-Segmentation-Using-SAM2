# Multi-Object Video Segmentation using SAM 2

An **interactive, transformer-based system** for **multi-object image and video segmentation** using **SAM 2 (Segment Anything Model 2)**.  
This project enables **prompt-based segmentation, memory-driven video tracking, and temporally consistent multi-object segmentation** without retraining.

---

# Project Overview

Traditional segmentation models process video frames independently, which leads to:

-  Flickering segmentation masks  
-  Loss of object identity between frames  
-  Poor temporal consistency  

This project overcomes these limitations by leveraging **SAM 2**, a **transformer-based segmentation framework with streaming memory**, enabling:

-  Accurate segmentation  
-  Stable tracking across frames  
-  Multi-object support  
-  No retraining required  

---

# Key Features

-  **Pixel-level multi-object segmentation**
-  **Prompt-based interaction** (points, bounding boxes, masks)
-  **Video object tracking with memory**
-  **Temporal consistency across frames**
-  **Near real-time performance**
-  **No retraining required**
-  **Transformer-based global context modeling**

---

#  System Architecture

## Core Components

- **Vision Transformer (ViT) Encoder** – Extracts deep image features  
- **Prompt Encoder** – Encodes user prompts (points, boxes, masks)  
- **Memory Module** – Stores object information across frames  
- **Mask Decoder** – Generates segmentation masks and IoU scores  

---

#  Tech Stack

| Category | Tools |
|--------|--------|
| **Language** | Python 3.10+ |
| **Framework** | PyTorch |
| **Libraries** | NumPy, OpenCV, Matplotlib, TorchVision |
| **Model** | SAM 2 (Pretrained) |
| **Environment** | Google Colab / Jupyter Notebook |
| **Hardware** | NVIDIA GPU (Recommended) |

---

#  Installation & Setup

## 1️⃣ Clone the Repository

```bash
git clone https://github.com/DoddaMeghana/Multi-Object-Segmentation-Using-SAM2.git
cd Multi-Object-Segmentation-Using-SAM2
```

## 2️⃣ Install Dependencies

```bash
pip install torch torchvision opencv-python numpy matplotlib
```

## 3️⃣ Download SAM 2

```bash
git clone https://github.com/facebookresearch/sam2.git
```

---

#  Usage

## 🖼️ Image Segmentation

- Provide an image  
- Add prompt (click / bounding box / mask)  
- Generate **pixel-level segmentation**

## 🎥 Video Segmentation & Tracking

- Initialize object with prompt on first frame  
- Track objects across frames using **memory module**  
- Generate **temporally consistent masks**

---

#  Results

**Performance Highlights:**

- 🔹 Accurate object boundaries  
- 🔹 Stable segmentation across frames  
- 🔹 Reduced identity switching  
- 🔹 Supports multiple objects simultaneously  

| Input | Objects | Temporal Stability | Output Quality |
|------|--------|-------------------|---------------|
| Image | Multiple | N/A | High |
| Video | Multiple | High | Stable Masks |

---

# 🔗 Project Demo Video

👉 Add your demo link here:  
[https://drive.google.com/file/d/19mL5IlmrvyoJfJkTDtWrc5eG1RHkeGF1/view?usp=drivesdk]

---

# 📁 Project Structure

```
.
├── sam2/
├── notebooks/
├── input_videos/
├── outputs/
├── README.md
└── requirements.txt
```

---

#  Applications

- Autonomous driving perception  
- Medical image segmentation  
- Video surveillance and tracking  
- Robotics vision systems  
- Video editing and VFX  

---
