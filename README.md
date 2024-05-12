
# Automatic Parking Space Detection

This project find outs the count of empty and occioped parking spaces in a car-parking-area using digital image processing techniques and opencv.


## Requirements

- OpenCV (Open Source Computer Vision Library)

- NUMPY library

- Pickle module
- CarparkingPos file 
- CarParking Mp4 video and image




## Methodology of the Project




- Objective Clarification:
   - Analyze a video (carPark.mp4) to detect parking space occupancy.
   
- Initialization:
   - Import necessary libraries: cv2, numpy, pickle.
   - Initialize variables: rectW, rectH, cap.
   
- Loading Parking Space Positions:
   - Load parking space positions from 'carParkPos' using Pickle.
   
- Frame Processing Loop:
   - Read each frame from the video (cap.read()).
   - Convert frame to grayscale, apply Gaussian blur, and adaptive thresholding.
   - Further enhance detected objects using median blur and dilation.
   
- Parking Space Detection:
   - Iterate through each parking space position.
   - Extract region of interest (ROI) from processed frame.
   - Count non-zero pixels in ROI to determine occupancy status.
   - Draw rectangles around parking spaces based on occupancy.
   
- Displaying Results:
   - Overlay processed frame with drawn rectangles.
   - Display number of vacant and total parking spaces on the frame.
   
- Video Playback and Control:
   - Continue processing frames until the video ends.
   - Display each frame for 10 milliseconds.
   
- Termination:
   - End processing once video playback ends.



![Capture1](https://github.com/Tonnydey/Automatic-Parking-Space-Detection/assets/150002822/2145d168-105e-4dec-8865-48a48197f0a4)

- Extracting the parking coordinates from Carparkinpos file. 
Then use this coordinates to process every car parking space individualy.
Implementing digital iamge processing techniques to find out the empty and occupied parking spaces.
drawing the results into the image.


## Application

- Smart Parking Management

- Parking Guidance Systems
- Security and Surveillance

- Traffic Flow Management


