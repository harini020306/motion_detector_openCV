# OpenCV Motion Detection

A simple real-time motion detection project built using Python, OpenCV, and Imutils.

## Features

* Captures live video using a webcam
* Detects movement by comparing video frames
* Highlights detected motion with a green rectangle
* Displays the status as **Normal** or **Motion Detected**
* Uses Gaussian Blur and image thresholding for better detection

## Technologies Used

* Python
* OpenCV
* Imutils

## How It Works

The program captures the first frame from the webcam and uses it as the reference frame.

Each new frame is then:

1. Converted to grayscale
2. Smoothed using Gaussian Blur
3. Compared with the first frame
4. Thresholded to identify differences
5. Dilated to improve the detected regions
6. Analyzed using contours
7. Marked with a rectangle when motion is detected

## Installation

Install the required libraries:

```bash
pip install opencv-python imutils
```

Or:

```bash
pip install -r requirements.txt
```

## Run the Project

```bash
python motion_detection.py
```

Allow the program to access your webcam.

Press **Q** to stop the program.

## Output

The webcam window displays:

* **Normal** – No significant movement detected
* **Motion Detected** – Movement detected in the camera frame

## Future Improvements

* Add motion detection timestamps
* Save images when motion is detected
* Add email or notification alerts
* Detect and track multiple moving objects
* Add person detection using AI/ML

## Author

Harini K
