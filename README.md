# Signals and Systems Project: Object Detection and Tracking (YOLO + CSRT/KCF/MOSSE)

This project delivers an advanced object detection and tracking pipeline designed for robust performance across various video scenarios. It seamlessly integrates the powerful YOLOv5 deep learning model for object detection with both established traditional tracking algorithms (CSRT, KCF, MOSSE) and a custom-built Kalman Filter-based tracker. This fusion approach aims to leverage the strengths of both detection (accurate localization) and tracking (smooth trajectories, handling occlusions) for enhanced video analysis.

---

##  Project Structure
- `main.py` – Main script to execute tracking
- `utils.py` – Helper functions for detection and tracking
- `requirements.txt` – Required Python packages
- `yolov5su.pt` – YOLOv5s custom model (not uploaded due to size)
- `SignalsSystemsProject.ipynb` – Main Google Colab notebook
- `data/` – Input video files
- `results/` – Output directory for processed videos
- `fusion/` – Contains CSRT, KCF, and MOSSE tracked videos

   ---

##  How to Run
open the SignalsSystemsProject.ipynb on google colab and start running each cell. 

   ---
## Requirements
Install dependencies with: 
