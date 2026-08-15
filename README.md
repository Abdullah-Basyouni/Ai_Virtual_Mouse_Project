# 🖱️ AI Virtual Mouse

A real-time **AI Virtual Mouse** that allows users to control their computer mouse using **hand gestures** through a webcam.

The project uses **MediaPipe Hand Tracking** to detect hand landmarks and **OpenCV** to process the webcam stream, then translates specific hand movements into mouse actions.

## 🚀 Project Idea

The goal of this project is to create a touch-free mouse interface using only:

* 📷 Webcam
* ✋ Hand gestures
* 🤖 MediaPipe
* 👁️ OpenCV
* 🐍 Python

Instead of using a physical mouse, the user can move the cursor and perform mouse actions using their hand.

## ✨ Features

* Real-time hand detection
* Hand landmark tracking using MediaPipe
* Control the mouse cursor using the index finger
* Left click using hand gestures
* Right click using hand gestures
* Smooth cursor movement
* Real-time webcam processing
* No physical mouse required

## 🛠️ Technologies Used

| Technology | Purpose                              |
| ---------- | ------------------------------------ |
| Python     | Main programming language            |
| OpenCV     | Webcam and image processing          |
| MediaPipe  | Hand detection and landmark tracking |
| NumPy      | Numerical operations                 |
| PyAutoGUI  | Controlling the system mouse         |

## 🧠 How It Works

The system follows this pipeline:

```text
Webcam
   ↓
OpenCV
   ↓
MediaPipe Hand Detection
   ↓
21 Hand Landmarks
   ↓
Gesture Detection
   ↓
Mouse Action
```

MediaPipe detects the hand and returns **21 landmarks** for each detected hand.

The landmarks are then used to determine:

* Finger positions
* Hand movement
* Distance between fingers
* Specific gestures

These gestures are mapped to computer mouse actions.

### 🖱️ Cursor Movement

The **index finger landmark** is used to control the mouse cursor.

The coordinates from the webcam frame are mapped to the computer screen coordinates.

```text
Camera Coordinates
       ↓
Coordinate Mapping
       ↓
Screen Coordinates
       ↓
Mouse Cursor
```

### 👆 Mouse Click

Specific finger configurations are detected to trigger mouse clicks.

For example, the distance between the **thumb** and **index finger** can be used to detect a clicking gesture.

## 📦 Installation

Clone the repository:

```bash
git clone https://github.com/Abdullah-Basyouni/Ai_Virtual_Mouse_Project.git
```

Navigate to the project directory:

```bash
cd Ai_Virtual_Mouse_Project
```

Install the required libraries:

```bash
pip install opencv-python mediapipe numpy pyautogui
```

## ▶️ Run the Project

Run the main Python file:

```bash
python main.py
```

Make sure your webcam is connected and accessible.

## 📁 Project Structure

```text
AI_Virtual_Mouse_Project/
│
├── main.py
├── README.md
├── requirements.txt
│
└── ...
```

## 🎯 Future Improvements

Some possible improvements for future versions:

* Add double-click gesture
* Add drag-and-drop gesture
* Add scrolling gestures
* Improve cursor smoothing
* Add left/right hand support
* Improve gesture recognition
* Add customizable gestures
* Reduce cursor latency
* Add a graphical user interface

## 👨‍💻 Author

**Abdullah Basyouni**

GitHub:
https://github.com/Abdullah-Basyouni

## ⭐ Project

If you find this project useful or interesting, feel free to ⭐ the repository.
