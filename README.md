# Air-Canvas

## Draw in the Air with Finger Using OpenCV & MediaPipe

The project uses **OpenCV** for computer vision, and **MediaPipe** for hand landmark detection. By detecting the landmarks on hand's knuckles, we can track our finger and convert our hand movements into on-screen drawings.

## Features

- **Draw in the air**: Can draw anything in the air using forefinger.
- **Hand detection**: Tracks one hand and identifies key landmarks to recognize drawing finger.
- **Real-time canvas**: Draws on a virtual canvas that updates in real time.
- **Customizable colors**: Changes the drawing ink with on-screen buttons.

## Algorithm Overview

1. **Capture frames**: Reads frames from webcam and converts them to HSV color space (for better color detection).
2. **Prepare canvas**: Initializes a blank canvas and create buttons for ink colors.
3. **Hand detection**: Use MediaPipe to detect hand landmarks, focusing on the forefinger for drawing.
4. **Track finger movements**: Stores the forefinger's coordinates across frames in an array to simulate drawing.
5. **Render drawing**: Uses OpenCV to draw the stored points on the canvas in real time.

### Requirements

- Python 3.12.3
- OpenCV
- NumPy
- MediaPipe
