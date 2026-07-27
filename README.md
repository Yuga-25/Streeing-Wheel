# 🎮 Virtual Steering Wheel

Control racing games using only your hands and a webcam. This project uses **MediaPipe** for real-time hand tracking and **OpenCV** for computer vision to simulate a virtual steering wheel. No physical steering wheel or controller is required.

---

## 📖 Overview

The Virtual Steering Wheel tracks both hands through your webcam and converts hand gestures into keyboard inputs. Hold both hands like you're gripping a steering wheel to accelerate and tilt your hands left or right to steer. Open both hands to brake.

---

## ✨ Features

- 🖐️ Real-time hand tracking using MediaPipe
- 🎥 Webcam-based gesture recognition
- 🎮 Controls any game that uses arrow keys
- 🚗 Steering based on hand tilt
- ⬆️ Accelerate with both fists
- ⬇️ Brake with both open hands
- 📊 Live steering angle and FPS display
- 🎨 Interactive HUD with virtual steering wheel
- ⚙️ Configurable sensitivity and camera settings

---

## 🛠️ Technologies Used

- Python 3
- OpenCV
- MediaPipe
- NumPy
- pynput

---

## 📂 Project Structure

```
Virtual-Steering-Wheel/
│
├── steering_wheel.py
├── requirements.txt
└── README.md
```

---

## 🚀 Installation

### 1. Clone the repository

```bash
git clone https://github.com/your-username/Virtual-Steering-Wheel.git
cd Virtual-Steering-Wheel
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

or

```bash
pip install mediapipe opencv-python pynput numpy
```

### 3. Run the project

```bash
python steering_wheel.py
```

Press **Q** to quit.

---

## 🎮 Controls

| Gesture | Action | Keyboard |
|----------|--------|----------|
| 👊 Both fists | Accelerate | ↑ Up Arrow |
| 👊 Tilt Left | Accelerate + Left | ↑ + ← |
| 👊 Tilt Right | Accelerate + Right | ↑ + → |
| 🖐 Both open hands | Brake | ↓ Down Arrow |
| 🖐 Tilt Left | Brake + Left | ↓ + ← |
| 🖐 Tilt Right | Brake + Right | ↓ + → |
| 👊🖐 One fist, one open | Neutral | No throttle |
| No hands detected | Release all keys | — |

---

## ⚙️ Configuration

The following settings can be changed at the top of `steering_wheel.py`:

| Setting | Description |
|----------|-------------|
| `CAMERA_INDEX` | Select webcam (0, 1, 2...) |
| `DEAD_ZONE_DEG` | Steering dead zone |
| `SOFT_ZONE_DEG` | Steering sensitivity |
| `FLIP_CAMERA` | Mirror camera feed |
| `GRACE_FRAMES` | Delay before releasing keys |
| `OPEN_FINGER_THRESH` | Fingers required to detect an open hand |

Customize these values to improve responsiveness for your setup.

---

## 🎯 Compatible Games

This project works with most games that use the **Arrow Keys**, including:

- Google Chrome Dinosaur Game
- Trackmania
- TORCS
- Hill Climb Racing (Browser)
- Browser Racing Games
- Other PC racing games with keyboard controls

---

## 🖥️ Requirements

- Python 3.9+
- Webcam
- Windows, macOS, or Linux

---

## 📸 Screenshots

Add screenshots or GIFs here to showcase the project.

Example:

```
screenshots/
├── gameplay.png
├── steering.png
└── demo.gif
```

---

## 🔮 Future Improvements

- Steering calibration
- Gesture customization
- Controller vibration support
- GUI settings panel
- Multiplayer support
- VR compatibility
- Steering smoothing improvements

---

## 👨‍💻 Developed By

**Yuga**

Diploma in Artificial Intelligence and Machine Learning

---

## 📄 License

This project is open-source and intended for educational and learning purposes. Feel free to use, modify, and improve it.
