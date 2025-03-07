# 🎛️ Gesture Volume Control using Hand Tracking

This project allows users to control the system volume using **hand gestures** detected through a **webcam**. It uses **OpenCV, MediaPipe, and PyCaw** to detect hand landmarks and adjust the system volume based on the distance between the **thumb** and **index finger**.

## 📌 Features
- 🎥 **Real-time hand tracking** using MediaPipe.
- ✋ **Gesture-based volume control** (move thumb and index finger closer/farther to decrease/increase volume).
- 🔊 **Real-time feedback** with a visual volume bar and percentage display.
- 🖥️ **Runs on Windows** (uses PyCaw for volume control).

## 🛠️ Technologies Used
- **Python**
- **OpenCV** (for capturing video and image processing)
- **MediaPipe** (for hand tracking)
- **NumPy** (for numerical operations)
- **PyCaw** (for system volume control on Windows)

## 📂 Project Structure

## 🚀 Installation & Setup
### **1️⃣ Install Dependencies**
Ensure you have **Python** installed. Install required libraries using:
```sh
pip install opencv-python mediapipe numpy pycaw comtypes

🎯 How It Works
Capturing Video from Webcam

cv2.VideoCapture(0) starts the webcam.
Frames are read and converted to RGB format.
Hand Tracking using MediaPipe

Detects hand landmarks and tracks movement.
Identifies thumb (ID: 4) and index finger (ID: 8).
Gesture-Based Volume Control

Calculates distance between thumb & index finger.
Maps the distance to system volume range.
Uses np.interp() to convert distance to volume levels.
Displaying Results

Shows a real-time volume bar and percentage.
Visualizes gesture tracking with drawn landmarks.
