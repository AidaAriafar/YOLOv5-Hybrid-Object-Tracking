# Signals and Systems Project: Object Detection and Tracking (YOLO + CSRT/KCF/MOSSE/custom-built Kalman Filter-based tracker)

This project delivers an advanced object detection and tracking pipeline designed for robust performance across various video scenarios. It seamlessly integrates the powerful YOLOv5 deep learning model for object detection with both established traditional tracking algorithms (CSRT, KCF, MOSSE) and a custom-built Kalman Filter-based tracker. This fusion approach aims to leverage the strengths of both detection (accurate localization) and tracking (smooth trajectories, handling occlusions) for enhanced video analysis.

---

##  Features

* **Hybrid Tracking Approach:** Combines state-of-the-art YOLOv5 detection with efficient tracking algorithms.

* **Multiple Tracker Support:**
    * **Traditional OpenCV Trackers:** CSRT, KCF, and MOSSE for diverse tracking characteristics.
    * **Custom Kalman Filter-based Tracker (`MyCustomTracker`):** A bespoke implementation for predictive and smooth tracking, particularly effective in multi-object scenarios.

* **Single and Multi-Object Tracking Modes:** Flexible operation for tracking one primary object or multiple objects simultaneously.

* **Performance Optimization:** Includes strategies (like sparse detection intervals) to significantly boost processing speed (FPS), especially for the custom tracker.

* **Configurable Detection:**
    * Adjustable **confidence threshold** for YOLOv5 detections.
    * Optional **target class filtering** to track specific object types (e.g., 'car', 'person').

* **Detailed Logging:** Provides informative console output during processing for better understanding and debugging.

* **Video Output:** Generates output video files with bounding boxes and track IDs.
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
It is highly recommended to run this project in a Google Colab environment due to the computational demands of YOLOv5 and the specific OpenCV/NumPy version requirements.
So just simply open the SignalsSystemsProject.ipynb on google colab and start running each cell. There's a title available above each cell giving a clue about what it does.

   ---
## Report
A detailed report is also available, providing clear explanations of the system architecture, fusion methodology, implementation choices, and results. It includes insights into how each tracking algorithm performs under different scenarios, along with visual comparisons and analysis.
This can be especially helpful for understanding the project’s signals and systems relevance and practical applications.

   ---
   
## Sample Outputs


###  Single-Object Tracking 
![Single-object tracking](sample%20images/single%20object%20tracking.png)

###  Multi-Object Tracking with custom-built kalman filter tracker
![Multi-object tracking](sample%20images/multi%20object%20tracking.png)
![Multi-object custom tracking](sample%20images/multi%20custom%20tracked%20video%20(8).gif)


  ---
   
## Contributors
* Aida Ariafar: https://github.com/AidaAriafar
* Kiarash Hamidieh: https://github.com/kiahmdh
* Amirali Entezam
  
