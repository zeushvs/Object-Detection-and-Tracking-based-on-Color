Color-Based Object Detection and Tracking:
This project implements real-time object detection and tracking using color calibration as the primary feature. 
The system begins by calibrating the target object's color range in HSV space, allowing for robust segmentation
under varying lighting conditions. Once calibrated, the object is continuously tracked using contour detection 
and a minimum enclosing circle, with a center dot to mark its position. This visual feedback not only aids in 
tracking but also enables spatial analysis based on the object's proximity and alignment within the frame.


Dynamic Movement Feedback System
To simulate basic directional control, the system interprets object movement relative to the camera. If the object
moves closer, the radius of the enclosing circle increases, triggering a "STOP" signal. Horizontal displacement is 
analyzed via the x-coordinate of the center dot—if it deviates from a predefined threshold, the system prints "LEFT" 
or "RIGHT" accordingly. This logic mimics rudimentary gesture-based navigation and can be extended for robotics, 
interactive interfaces, or embedded vision systems. The project is built using OpenCV and Python, and serves as a 
foundational module for color-based tracking applications.
