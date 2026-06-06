#  AI-Based Smart Driver Monitoring System

A real-time Driver Monitoring System developed using **Python, OpenCV, and MediaPipe Face Mesh** to detect **drowsiness, distraction, head-down posture, and inattentive driving behavior**. The system continuously analyzes facial landmarks, eye movements, gaze direction, and head position to improve driver safety through intelligent monitoring and audio alerts.

##  Features

* Eye Aspect Ratio (EAR) based drowsiness detection
* Real-time gaze tracking (Left, Right, Center)
* Head-down posture detection
* Priority-based audio alert system
* Fatigue score monitoring
* Blink counting
* Inattentive time tracking
* CSV event logging
* Real-time performance monitoring (FPS)
* User-specific calibration for improved accuracy

## Technologies Used

* Python
* OpenCV
* MediaPipe Face Mesh
* NumPy
* Pygame
* Git & GitHub

## Project Structure

```text
AI-Based-Smart-Driver-Monitoring-System/
│
├── main.py
├── detection.py
├── state.py
├── audio.py
├── logger.py
├── config.py
├── fatigue_log.csv
├── sounds/
│   ├── drowsy.mp3
│   ├── left.mp3
│   ├── right.mp3
│   └── down.mp3
└── README.md
```

## Installation

### Clone Repository

```bash
git clone https://github.com/Dev252001/AI-Based-Smart-Driver-Monitoring-System.git
cd AI-Based-Smart-Driver-Monitoring-System
```

### Install Dependencies

```bash
pip install opencv-python mediapipe numpy pygame
```

## Run Project

```bash
python main.py
```

Press **Q** to exit the application.

## Working Pipeline

```text
Webcam Input
      ↓
OpenCV Video Capture
      ↓
MediaPipe Face Mesh
      ↓
Facial Landmark Extraction
      ↓
EAR + Gaze + Head Analysis
      ↓
Driver State Detection
      ↓
Audio Alerts & Event Logging
      ↓
Real-Time Dashboard
```

## Driver States Detected

| State             | Description                                   |
| ----------------- | --------------------------------------------- |
| ACTIVE            | Driver is attentive                           |
| DROWSY            | Eye closure detected for a prolonged duration |
| LEFT              | Driver looking left                           |
| RIGHT             | Driver looking right                          |
| DOWN              | Driver's head tilted downward                 |
| FACE NOT DETECTED | Face not visible to the camera                |

## Displayed Metrics

* Eye Aspect Ratio (EAR)
* Fatigue Score
* Blink Count
* Inattentive Duration
* Frames Per Second (FPS)
* Current Driver State

## Future Improvements

* Machine Learning based fatigue prediction
* Driver identity recognition
* Mobile application integration
* Cloud-based event storage
* Advanced behavioral analysis
* Night vision support

## Sample Outputs

* Active Driver Monitoring
* Drowsiness Detection
* Left/Right Distraction Detection
* Head-Down Detection
* Face Not Detected Warning

## Author

**Devashish Pandey**

Bachelor of Computer Applications (BCA)
Galgotias University
