# 🎬 Video Frame Analysis

Automated video processing pipeline that extracts, analyses, and classifies individual frames from video files — enabling object detection, motion analysis, and visual data extraction at scale.

## 🛠️ Tech Stack
- **Python 3.x** — core language
- **OpenCV (cv2)** — video capture, frame extraction, image processing
- **NumPy** — array operations on image data
- **Matplotlib** — frame visualization and result plotting
- **Jupyter Notebook** — interactive development

## 📌 What It Does
- Reads video files and extracts frames at configurable intervals (every N frames)
- Preprocesses frames: grayscale conversion, resizing, noise reduction
- Detects motion between consecutive frames using frame differencing
- Identifies key frames — frames with significant visual change
- Saves extracted frames as images for downstream ML or manual review
- Generates frame-level analysis report (motion score, brightness, contrast)

## 🧠 Key Concepts Demonstrated
- Video as a sequence of images — temporal processing
- Frame differencing for motion detection (absolute difference + threshold)
- Contour detection for identifying regions of interest
- Histogram analysis for brightness and exposure consistency
- Batch image processing pipeline

## 🚀 How to Run
```bash
git clone https://github.com/DhaaraniPushpam/Video-Frame-Analysis
cd Video-Frame-Analysis
pip install opencv-python numpy matplotlib jupyter
jupyter notebook
```

Configure the target video:
```python
VIDEO_PATH = "your_video.mp4"
FRAME_INTERVAL = 30   # extract every 30th frame
MOTION_THRESHOLD = 25  # pixel difference to flag as motion
```

## 📂 Output
```
output/
├── frames/          # extracted frame images
├── keyframes/       # high-motion / significant frames only
└── analysis.csv     # per-frame metrics
```

## 🔍 Extensions & Applications
- Feed extracted frames into a CNN for object classification
- Use for surveillance video analysis
- Pre-processing step for video ML datasets
- Quality control in video production pipelines

---
*Demonstrates computer vision fundamentals and video data engineering — applicable to AI/ML and media tech roles.*
