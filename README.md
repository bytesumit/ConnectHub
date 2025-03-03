# Virtual Painter 🎨

## Introduction
Virtual Painter is a computer vision-based drawing application that allows users to draw using hand gestures. It leverages **MediaPipe** for hand tracking and **OpenCV** for rendering drawings on a digital canvas. Users can switch between different tools like a brush, line, rectangle, circle, and eraser simply by pointing at the tool panel.

## Features 🚀
- Hand gesture-based drawing 🖐️
- Multiple drawing tools: **Brush, Line, Rectangle, Circle, Eraser** ✏️
- Real-time hand tracking using **MediaPipe**
- Works with a webcam 📷

## Installation 🛠️
Ensure you have **Python 3.7 - 3.10** installed. If you are using **Python 3.11+**, downgrade to 3.10 as MediaPipe doesn't support higher versions yet.

### 1️⃣ Create a Virtual Environment (Recommended)
```sh
python3 -m venv venv
```
Activate the virtual environment:
- **Windows**: `venv\Scripts\activate`
- **Mac/Linux**: `source venv/bin/activate`

### 2️⃣ Install Dependencies
```sh
pip install mediapipe opencv-python numpy
```

## Usage 🏃‍♂️
1. Run the Python script:
   ```sh
   python virtual_painter.py
   ```
2. The camera feed will open with a tool selection panel.
3. Move your index finger over the tool panel to choose a drawing tool.
4. Start drawing on the canvas using hand gestures.
5. Press **Esc** to exit the application.

## Tools 🛠️
| Tool | Gesture |
|------|---------|
| 🖌 Draw | Index finger up & moving |
| ➖ Line | Raise index finger & hold |
| ▭ Rectangle | Raise index finger & hold |
| 🔵 Circle | Raise index finger & hold |
| 🧼 Erase | Move finger while in erase mode |

## Requirements 📝
- Python 3.7 - 3.10
- MediaPipe
- OpenCV
- NumPy
- Webcam

## Troubleshooting ⚠️
- **ModuleNotFoundError: No module named 'mediapipe'**
  - Ensure Python is in the correct version (3.7 - 3.10)
  - Try `pip install mediapipe --no-cache-dir`

- **Camera not opening?**
  - Check if another application is using the webcam.
  - Try changing the camera index in `cv2.VideoCapture(0)` to `cv2.VideoCapture(1)`.

## Contributing 💡
Feel free to improve this project by adding:
- Color selection 🎨
- Thickness control 🖊️
- Save drawings feature 📁

---
Happy coding! 🚀

