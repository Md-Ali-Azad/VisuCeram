# VisuCeram: A Comprehensive Dataset for Sanitary Ware Ceramic Defect Detection

## 📄 Related Publication

This repository contains the **official dataset and YOLO-based implementation models** for the paper:

**“VisuCeram: A Comprehensive Dataset for Sanitary Ware Ceramic Defect Detection with YOLO Models and Benchmarking”**  
Published by IEEE  

🔗 Paper link: https://ieeexplore.ieee.org/abstract/document/11367538/

---

## 🧱 Repository Overview

In the sanitary ware ceramics industry, visual quality inspection is essential to ensure product quality and reduce manufacturing defects. Manual inspection is:

- Labor-intensive  
- Time-consuming  
- Prone to human error  

Additionally, ceramic products present unique challenges such as:

- Complex surface geometries  
- Highly reflective glaze surfaces  

To address these challenges, we introduce **VisuCeram**, a publicly available dataset specifically designed for **ceramic defect detection using YOLO-based object detection models**.

---

## 📊 Dataset Information

The VisuCeram dataset contains:

- **3,265 high-resolution images**
- **7 defect categories**, including:
  - Surface cracks  
  - Glaze imperfections  
  - Other ceramic surface defects  

### 📦 Available Dataset Versions

Two versions of the dataset are provided:

#### 1️⃣ VisuCeram-1000x1000.zip
- Image resolution: **1000 × 1000 pixels**
- High-quality images
- Intended for visualization and detailed inspection

#### 2️⃣ VisuCeram-500x500-labelled.zip
- Image resolution: **500 × 500 pixels**
- Used for all experiments in the paper
- Fully annotated with:
  - Precise bounding boxes  
  - YOLO text-format labels  
- Annotations created using Label Studio  
- Includes detailed class labels for each defect type  

This second version is optimized for direct integration with YOLO-based frameworks.

---

## 🤖 YOLO Models

The repository includes the following YOLO-based architectures:

- YOLOv3-light  
- YOLOv4-light  
- YOLOv7-light  
- VisuCeramNet (proposed model)  

All models are located inside the **`YOLO models`** folder.

### 📈 Benchmark Results (mAP)

| Model | mAP (%) |
|-------|---------|
| YOLOv4-light | **87.30%** |
| YOLOv7-light | 46.56% |
| VisuCeramNet | 46.10% |
| YOLOv3-light | 41.74% |

YOLOv4-light achieved the best performance on the VisuCeram dataset.

---

## ⚙️ How to Run the Models

To train and test the models, you must use the Darknet framework:

🔗 Darknet repository: https://github.com/AlexeyAB/darknet

### Steps:

1. Clone and build the Darknet framework.
2. Place the dataset and model configuration files appropriately.
3. Use the provided YOLO configuration files inside the `YOLO models` folder.
4. Train or test using Darknet commands.

Please refer to the Darknet documentation for detailed installation and usage instructions.

---

## 🎯 Purpose of This Repository

- Provide a benchmark dataset for ceramic defect detection  
- Support research in industrial visual inspection  
- Enable comparison of lightweight YOLO-based detection models  
- Promote automation in the sanitary ware ceramics industry  

---

## 📌 Citation

If you use this dataset or code in your research, please cite:

```bibtex
@inproceedings{azad2025visuceram,
  title={VisuCeram: A Comprehensive Dataset for Sanitary Ware Ceramic Defect Detection with YOLO Models and Benchmarking},
  author={Azad, Md Ali and Nahid, Md Mahadi Hasan},
  booktitle={2025 IEEE 7th International Conference on Sustainable Technologies For Industry 5.0 (STI)},
  pages={1--6},
  year={2025},
  organization={IEEE}
}
```

---
