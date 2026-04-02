 # Real-Time Object Detection & Tracking System

A real-time object detection and tracking system built with YOLOv8 and OpenCV.
Detects 80 COCO classes via webcam, tracks objects with persistent IDs using
ByteTrack, and counts unique objects crossing a defined line zone.

## Features
- Real-time detection at 30+ FPS (GPU) using YOLOv8n
- Persistent object tracking with ByteTrack (unique IDs per object)
- Line-crossing counter (IN/OUT) for people and vehicles
- FPS display and live class totals sidebar
- CSV telemetry logging (timestamp, class, confidence, bounding box)
- Video output saved to MP4

## Tech Stack
- YOLOv8 (Ultralytics)
- OpenCV
- Supervision
- PyTorch (CUDA)
- Python 3.10+

## Setup
1. Clone the repo
2. Install dependencies
   pip install -r requirements.txt
3. Run
   jupyter notebook real_time_detection_system.ipynb

## Notes
- YOLOv8n weights download automatically on first run
- Adjust LINE_START and LINE_END coordinates to match your webcam resolution
