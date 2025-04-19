# 🚨 Accident & Disaster Detection Model using YOLOv11
This repository contains object detection models trained to detect **accidents** and **natural disasters** using YOLOv11. The system is part of a broader initiative to improve real-time disaster and accident response through automated monitoring of CCTV feeds. The model training includes detection for car collision, fire, flood, and landslide.

### 🧠 Model Descriptions
- **custom.pt**: A custom YOLOv11-based model trained on 18,753 labeled images across 5 classes (collision, fire, smoke, flood, landslide). Designed specifically for accident and disaster detection using CCTV footage.
- **yolov11n.pt**: A pre-trained YOLOv11 nano model trained on the COCO dataset. Lightweight and optimized for general-purpose object detection with high inference speed, but not tailored for disaster-specific scenarios.

## Data Balance Summary
---------------------------------------------------------
Collision
📊 Dataset Split Summary
Total data: 6251
Train data: 5001 (80.00%)
Valid data: 1250 (20.00%)
✅ The dataset is approximately balanced (80/20 split).

---------------------------------------------------------
Fire
📊 Dataset Split Summary
Total data: 6252
Train data: 5001 (79.99%)
Valid data: 1251 (20.01%)
✅ The dataset is approximately balanced (80/20 split).

---------------------------------------------------------
Flood
📊 Dataset Split Summary
Total data: 3125
Train data: 2500 (80.00%)
Valid data: 625 (20.00%)
✅ The dataset is approximately balanced (80/20 split).

---------------------------------------------------------
Landslide
📊 Dataset Split Summary
Total data: 3125
Train data: 2500 (80.00%)
Valid data: 625 (20.00%)
✅ The dataset is approximately balanced (80/20 split).

🚗 Collision: 6251
🔥 Fire: 6252
🌊 Flood: 3125
🪨 Landslide: 3125
🧮 Overall Total: 18,753 images

Yolo Model Metrics

## 📈 Model Performance Metrics (Post-Training)

| Model     | Precision | Recall | mAP50 | mAP50-95 |
|-----------|-----------|--------|--------|-----------|
| **All**       | 67%       | 58%    | 61%    | 41%       |
| **Collision** | 89%       | 91%    | 95%    | 85%       |
| **Fire**      | 74%       | 64%    | 72%    | 33%       |
| **Smoke**     | 58%       | 34%    | 43%    | 18%       |
| **Flood**     | 83%       | 64%    | 69%    | 57%       |
| **Landslide** | 29%       | 36%    | 24%    | 14%       |