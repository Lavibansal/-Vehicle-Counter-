# Vehicle Counter with OpenCV
This project implements a vehicle counting system using C++ and OpenCV. It uses background subtraction to detect moving vehicles in a video, highlights them with bounding boxes, and counts them as they pass a designated line.

# Requirements
OpenCV (version 3.4 or higher recommended)
C++11 or higher
Installation
Install OpenCV (skip if already installed):

For Windows, download the OpenCV installer and follow the installation steps.
For Linux, use the following command:
bash
Copy code
sudo apt-get install libopencv-dev
Clone the Repository:

bash
Copy code
git clone <repository-url>
cd <repository-folder>
Compile the Program: Use the following command to compile:

bash
Copy code
g++ vehicle_counter.cpp -o vehicle_counter `pkg-config --cflags --libs opencv4`
Usage
Place the video file (video.mp4) in the same directory as the compiled program.

Run the program:

bash
Copy code
./vehicle_counter
The program will display the video with detected vehicles and a counter indicating the number of vehicles that have crossed a designated line.

Press 'q' to quit the program.

How It Works
Background Subtraction: The system applies background subtraction to isolate moving objects (vehicles) in the frame.
Contour Detection: It detects the contours of moving vehicles and draws bounding boxes around them.
Counting Line: A line is drawn, and vehicles crossing this line are counted.
Display: The vehicle count is displayed on the video screen, and each detected vehicle is highlighted with a bounding box.
