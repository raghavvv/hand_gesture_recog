# Hand Gesture Recognition with OpenCV

This project is a Python-based hand gesture recognition system using OpenCV and NumPy. The code captures video from a webcam, detects a hand within a specified region, and recognizes gestures based on the number of convexity defects (finger gaps). When a gesture with five fingers extended is detected, it simulates a spacebar press using `pyautogui`—for example, to make a character "jump" in a game.

## Features

- Real-time hand detection using color segmentation in HSV space.
- Morphological operations to reduce noise and improve contour detection.
- Convex hull and convexity defect analysis to count extended fingers.
- Automated keyboard interaction (presses the spacebar) when a specific gesture is recognized.
- Visual feedback with bounding boxes, contours, and gesture status on the video feed.

## Requirements

- Python 3.x
- OpenCV (`cv2`)
- NumPy
- PyAutoGUI

Install dependencies with:
```bash
pip install opencv-python numpy pyautogui
```

## Usage

1. Run the notebook or script.
2. Allow webcam access.
3. Place your hand inside the green rectangle on the video feed.
4. Extend all five fingers to trigger a spacebar press (e.g., to "jump" in a game).
5. Press `q` to exit the application.

## Notes

- The gesture detection is based on skin color segmentation and may require good lighting and a plain background for best results.
- The region of interest is fixed at coordinates (200, 200) to (400, 400) in the webcam frame.
- You can modify the gesture logic or region as needed for your application.

---

This was done as a part of the project for Computer Vision in NIIT University in collab with Tulika Arun, Mohammad Ibrahim and Vaasu Sohee
