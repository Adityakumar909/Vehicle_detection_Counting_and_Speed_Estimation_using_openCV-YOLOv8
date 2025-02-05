![th1](https://github.com/AarohiSingla/Speed-detection-of-vehicles/assets/60029146/139d8cc9-32ab-4777-89d8-cb179c39fedd)
# Vehicle Detection and Speed Estimation using OpenCV & YOLOv8

## Overview
This project uses OpenCV and YOLOv8 to detect and track vehicles in a video feed, estimate their speed, and count the number of vehicles moving in different directions. The system processes frames from a video, identifies vehicles, tracks their movement across predefined lines, and calculates speed based on the time taken to cross a fixed distance.

## Features
- Vehicle detection using YOLOv8
- Object tracking with a custom tracker
- Speed estimation of vehicles
- Counting vehicles moving up and down
- Frame-by-frame result saving and video output generation

## Installation
To set up and run the project, follow these steps:

### Prerequisites
Ensure you have Python 3.8+ installed. You also need to install the required dependencies.

### Steps
```sh
# Clone this repository
git clone https://github.com/yourusername/vehicle-detection-opencv.git
cd vehicle-detection-opencv

# Install dependencies
pip install -r requirements.txt

# Download YOLOv8 model weights
wget https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8s.pt
```

## Usage
Run the main script to process the input video:
```sh
python main.py
```

### Input Video
Ensure that the video file (`highway.mp4`) is placed in the project directory. You can modify the script to use a different video file.

## Project Structure
```
vehicle-detection-opencv/
│── detected_frames/    # Stores processed frames with detections
│── output.avi          # Processed output video
│── tracker.py          # Custom object tracking module
│── main.py             # Main script for vehicle detection & tracking
│── README.md           # Project documentation
│── requirements.txt    # List of dependencies
│── yolov8s.pt          # YOLO model weights
```

## Results
The output will be displayed in real-time and saved as a processed video (`output.avi`). Frames with detected vehicles will be stored in the `detected_frames/` directory.

## Dependencies
This project requires the following Python libraries:
```sh
opencv-python
pandas
ultralytics
```
Install dependencies using:
```sh
pip install -r requirements.txt
```

## Acknowledgments
- [Ultralytics YOLO](https://github.com/ultralytics/ultralytics) for object detection
- OpenCV for image processing

## License
This project is licensed under the MIT License. See `LICENSE` for details.

## Contact
For any questions or issues, feel free to open an issue or contact me at `your.email@example.com`.

---
**Author:** Your Name  
**GitHub:** [yourusername](https://github.com/yourusername/)

