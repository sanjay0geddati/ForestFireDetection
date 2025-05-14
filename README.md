# ForestFireDetection
This project demonstrates a machine vision-based approach for detecting forest wildfires using video analysis. It integrates color features, motion detection, and OpenCV techniques to detect fire in videos, particularly those captured by UAVs (drones).

🧠 Project Overview
The application is built using Python's tkinter for GUI and OpenCV for image processing. It allows users to:

Upload a forest surveillance video.

Process the video to detect fire using HSV color thresholds.

Analyze motion between video frames to reinforce detection accuracy.

🖥️ Features
GUI for uploading videos and running detection.

Fire detection based on HSV color space filtering.

Motion detection using frame differencing and contour analysis.

Real-time video display with fire detection labels.


🛠️ Requirements
Install the following Python packages:

pip install numpy opencv-python


▶️ How to Run
Make sure you have Python installed (version 3.x).

Place your test video in the UAV_Videos/ directory.

Run the application:

bash
Copy code
python b92b02a5-b753-49d9-ad93-c961c2455cda.py
Use the GUI to:

Upload a video.

Start the detection process.

View live results in the popup video windows.

🎯 Detection Approach
🔶 Color Feature Detection
* Detects regions in HSV color space that match the fire's hue range.

🔁 Motion Detection
* Grayscale conversion and Gaussian blur are applied to frames.
* Frame differencing identifies motion.
* Thresholding and dilation help extract contours indicating motion regions.

📝 Note:-
* Fire detection is threshold-based and may be sensitive to lighting conditions.

* Motion detection is basic and doesn't track specific fire patterns or object identities.
