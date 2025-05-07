# 🖐️ Virtually-Mouse-control-by-hand-gesture

Control your mouse with just your hand using your webcam!

This Python-based project leverages MediaPipe, OpenCV, and pyautogui to track your hand and perform actions like moving the cursor, clicking, double-clicking, and taking screenshots — all using intuitive finger gestures.


[result output](https://github.com/user-attachments/assets/b56813fe-b1cf-45d5-8b8e-3a6a44208b05)

for know more about MediaPipe : https://ai.google.dev/edge/mediapipe/solutions/vision/hand_landmarker

![mediapipe](https://github.com/user-attachments/assets/e6d374ca-38c8-4b85-bdb3-4fd914bd2989)


## 🚀 Features

🖱️ Move Cursor – Control mouse movement with your index finger

👈 Left Click – Pinch gesture for left click

👉 Right Click – Reverse pinch for right click

👆 Double Click – Combine left and right click gesture

📸 Screenshot – Take screenshots with a specific hand pose

## 🧠 How It Works

Uses MediaPipe to detect and track hand landmarks in real-time

Calculates distances and angles between finger joints to recognize gestures

Translates gestures into mouse actions via pynput and pyautogui

Supports single-hand interaction for simplicity and speed

## 🧰 Dependencies


pip install opencv-python mediapipe pyautogui pynput

Make sure util.py contains functions like:

get_angle – returns the angle between 3 landmarks

get_distance – returns the distance

## 🎮 Usage

python hand_mouse_control.py

Ensure your webcam is active

Use gestures in front of the camera

Press q to quit the app

## 📷 Sample Gesture Map

Gesture	Action

Pinch index & thumb	Move mouse

👆 Index tip bent	Left click

👉 Middle tip bent	Right click

Both index & middle bent	Double click

Fingers close + angles aligned	Take Screenshot

