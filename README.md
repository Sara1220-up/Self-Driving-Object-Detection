# YOLOv8 + Norfair: Object Detection, Tracking, and Movement Analysis

This project demonstrates how to detect and track objects using [Ultralytics YOLOv8](https://github.com/ultralytics/ultralytics) and [Norfair](https://github.com/tryolabs/norfair), with real-time movement analysis.

## 🔍 Features
- Object detection using YOLOv8
- Object tracking using Norfair
- Movement analysis (speed & direction)
- COCO dataset model evaluation

---

## 📦 Setup

1. Clone this repository:
```bash
git clone https://github.com/YOUR_USERNAME/yolov8-norfair-object-tracking.git
cd yolov8-norfair-object-tracking

##
2. Create a virtual environment:
python -m venv venv
source venv/bin/activate

3. Install the dependencies:
pip install -r requirements.txt

🚀 Usage
To run the full detection + tracking + movement analysis pipeline:
python src/main.py --image assets/sample_image.png --model models/yolov8n.pt
This will save the result image with bounding boxes and print movement information in the console.

🧪 Model Evaluation
To evaluate model accuracy using COCO dataset:
from ultralytics import YOLO
model = YOLO('yolov8n.pt')
model.val(data='coco.yaml')


