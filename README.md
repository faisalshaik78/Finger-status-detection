# Finger Status Detection 🖐️

A Python computer-vision project that detects hands, tracks finger landmarks, identifies finger positions, and supports virtual drawing using a webcam.

## Overview

The application uses **MediaPipe**, **OpenCV**, and **NumPy** to track hand landmarks in real time. It can analyse finger positions, count raised fingers, and let you draw on a virtual canvas with your index fingertip.

This repository is maintained by **Shaik Faisal** as a learning and portfolio project. The original implementation is based on the work by [Shahid Azam](https://github.com/shahidazam2020-oss), with credit retained.

## Features

- Detect up to two hands using a webcam
- Track 21 landmarks on each detected hand
- Analyse finger positions and show **Up / Down** status
- Count raised fingers
- Identify bent fingers using joint angles
- Draw on a virtual canvas with the index fingertip
- Select colours and clear the canvas

## How It Works

1. Captures frames from the webcam.
2. Detects hands and their landmarks.
3. Analyses finger joints and estimates finger status.
4. Displays the tracking information on the video.
5. Uses the index fingertip for virtual drawing.

## Tech Stack

- **Python** — application logic
- **OpenCV** — webcam, image processing, and drawing
- **MediaPipe** — hand landmark detection
- **NumPy** — canvas and array operations
- **Math** — joint-angle calculations

## Run Locally

### 1. Clone the repository

```bash
git clone https://github.com/faisalshaik78/Finger-status-detection.git
cd Finger-status-detection
```

### 2. Create and activate a virtual environment

```bash
python -m venv venv
venv\\Scripts\\activate
```

### 3. Install dependencies

```bash
pip install opencv-python numpy mediapipe
```

### 4. Start the application

```bash
python hand-tracking.py
```

You'll need Python installed and a webcam. The MediaPipe model may be downloaded during the first run.

## Keyboard Controls

| Key | Action |
|---|---|
| `T` | Toggle hand tracking |
| `D` | Toggle drawing |
| `C` | Clear the canvas |
| `Q` | Quit |

## Project Structure

```text
Finger-status-detection/
├── hand-tracking.py
├── hand_landmarker.task
└── README.md
```

*The structure above is a simplified overview; additional files may be present in the repository.*

## Developer

**Shaik Faisal**  
Software Developer | Python | Computer Vision | AI & ML  
Hyderabad, India

[GitHub Profile](https://github.com/faisalshaik78)

## Acknowledgements

Original project implementation by [Shahid Azam](https://github.com/shahidazam2020-oss). This repository retains attribution to the original work.

---

Suggestions and improvements are welcome.
