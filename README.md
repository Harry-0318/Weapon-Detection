# Gun Detection with OpenCV

This project implements a real-time gun detection system using OpenCV and a Haar cascade classifier. It uses a webcam feed to detect the presence of guns in the video stream and provides visual feedback by marking detected guns with rectangles.

## Features
- Detects guns in a live video stream.
- Draws rectangles around detected guns.
- Displays the video stream with detection results.
- Prints a message indicating whether guns were detected upon exiting.

## Requirements
- Python 3.x
- OpenCV library
- imutils library
- Pre-trained Haar cascade XML file for gun detection (`cascade.xml`) is given in the repository

## Installation
1. Install Python and the required libraries:
   ```bash
   pip install opencv-python opencv-python-headless opencv-contrib-python imutils numpy
   ```
2. Ensure you have a compatible Haar cascade XML file for gun detection named `cascade.xml` in the same directory as the script.

## Usage
1. Run the script:
   ```bash
   python main.py
   ```
2. Press the `q` key to quit the video stream.

## Output
- The script displays the live video feed with rectangles drawn around detected guns.
- A message is printed to the console indicating whether guns were detected during the session.

## Notes
- The detection accuracy depends on the quality of the `cascade.xml` file.
- Ensure proper lighting conditions for better detection performance.
- Modify `minSize` in `detectMultiScale` for detecting guns of different sizes.
