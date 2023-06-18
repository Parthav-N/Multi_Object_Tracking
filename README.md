# Multi_Object_Tracking

This project is a multi-object tracking system that detects and tracks objects in a video stream using computer vision techniques. It utilizes the OpenCV library and implements the Euclidean distance-based tracking algorithm.

## Features

* Object detection using a background subtraction algorithm (cv2.createBackgroundSubtractorMOG2) to extract foreground objects from the video stream.
* Object tracking based on the Euclidean distance between the centroids of detected objects in consecutive frames.
* Real-time visualization of the tracked objects, including bounding boxes and unique IDs.

## Dependencies

* Python 3.x
* OpenCV (cv2)

## Installation

1. Clone the repository:
     ```git clone https://github.com/your-username/your-repository.git```
2. Install the required dependencies. Assuming you have Python and pip installed, run the following command:
     ```pip install opencv-python```

## Usage

1. Place the video file you want to analyze in the project directory.
2. Update the cap variable in the main file (main.py) with the path to your video file: ```cap = cv2.VideoCapture("your-video-file.mp4")```
3. Run the main file: ```python main.py``` The application will start processing the video and display the results in separate windows for the region of interest (ROI), the original frame, and the binary mask.
4. Press the 'Esc' key to exit the application.

## Customization

* Region of Interest (ROI): Adjust the coordinates in the roi variable within the main file to define the area where objects should be detected and tracked.

* Object Size Threshold: Modify the area threshold value in the main file to change the minimum size of detected objects. Objects smaller than this threshold will be ignored.
