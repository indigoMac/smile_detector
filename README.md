# Real-Time Face and Smile Detection
This repository contains a Python project that leverages OpenCV to perform real-time face, eye, and smile detection using a webcam. It utilizes Haar Cascades, a popular method for object detection in computer vision.

## Project Description
The script uses pre-trained Haar cascade models to detect facial features. The cascades process video frames in real-time to identify and mark faces, eyes, and smiles. Each detected face and eye is highlighted with a rectangle overlay in the video feed, and smiles trigger a text alert on-screen.

## Features
- Face Detection: Detects human faces within the video frame and marks them with blue rectangles.
- Eye Detection: Identifies eyes within the detected faces, marking each with green rectangles.
- Smile Detection: Recognizes smiles and not only marks them with red rectangles but also displays a message "Smile Detected!" on the screen.

## How It Works
- Library Importation: Utilizes OpenCV (cv2), a powerful library for computer vision tasks.
- Cascade Loading: Loads three different Haar cascades for detecting faces, eyes, and smiles.
- Detection Function: Defines a function detect() that:
  * Converts video frames to grayscale (necessary for Haar cascade detection).
  * Applies the face cascade to detect faces.
  * Applies the eye and smile cascades within each detected face to find eyes and smiles respectively.
  * Annotates the original frame with rectangles and text based on detection results.
- Webcam Feed Processing: Captures video feed from the webcam, processes each frame in the detect() function, and displays the annotated video in real time.
- User Interaction: Allows the user to quit the application by pressing 'q'.

## Setup and Running the Project
To run this project, you will need to have Python and OpenCV installed. Clone this repository and execute the script in a Python environment where OpenCV is installed. Make sure to place the Haar cascade files in the same directory as the script or update the path in the script accordingly.

```bash
python smile_detector.py
```

## Requirements
- Python 3.x
- OpenCV library

## License
This project is open-source and available under the MIT License.

# Contributions
Contributions are welcome! Please open an issue to discuss proposed changes or open a pullback request.
