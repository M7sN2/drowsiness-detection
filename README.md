#  Sleep Detector using OpenCV & MediaPipe

This is a simple real-time Python project that uses **MediaPipe** and **OpenCV** to detect if a person is falling asleep, based on whether their eyes remain closed for a certain duration.

##  Features

- Real-time webcam feed monitoring
- Eye detection using **MediaPipe FaceMesh**
- Calculates **Eye Aspect Ratio (EAR)** to determine eye closure
- Detects if person is likely sleeping (e.g., eyes closed for 20+ frames)
##  Requirements

Install the dependencies:

```bash
pip install opencv-python mediapipe numpy
```

## How It Works
- The system detects eye landmarks.
- Calculates the Eye Aspect Ratio (EAR).
- If the EAR stays below a threshold (< 0.2) for several consecutive frames (e.g., 20), it assumes the person is asleep.

  ## How to run
  ```
  python sleep_detector.py
  ```
  Press q to quit.





