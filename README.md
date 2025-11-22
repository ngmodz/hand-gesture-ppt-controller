# Hand Gesture PPT Controller 🖐️📽️

A Python-based application that allows you to control PowerPoint presentations using hand gestures captured through your webcam. Navigate slides and draw annotations without touching your keyboard or mouse!

## 🚀 Features

- **Gesture-based Navigation**: Control slides with simple hand gestures
- **Real-time Drawing**: Draw annotations directly on slides using finger gestures
- **Webcam Integration**: Uses your computer's camera to detect hand movements
- **Visual Feedback**: Live preview of your hand gestures and slide annotations

## 🎯 Hand Gestures

| Gesture | Action | Description |
|---------|--------|-------------|
| 👍 **Thumbs Up** | Previous Slide | Navigate to the previous slide |
| 🤙 **Pinky Up** | Next Slide | Navigate to the next slide |
| ✌️ **Index + Middle Finger** | Pointer Mode | Show a red pointer on the slide |
| ☝️ **Index Finger Only** | Drawing Mode | Draw annotations on the current slide |
| 🤟 **Index + Middle + Ring** | Erase | Remove the last drawn annotation |

## 📋 Prerequisites

- Python 3.7 or higher
- Webcam/Camera
- Presentation images in PNG format

## 🛠️ Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/ngmodz/hand-gesture-ppt-controller.git
   cd hand-gesture-ppt-controller
   ```

2. **Install required dependencies**
   ```bash
   pip install opencv-python
   pip install cvzone
   pip install numpy
   ```

## 📁 Setup

1. Place your presentation slides (as PNG images) in the `Presentation` folder
2. Name your slides sequentially (e.g., `1.png`, `2.png`, `3.png`, etc.)
3. Ensure your webcam is connected and working

## 🎮 Usage

1. **Run the application**
   ```bash
   python final.py
   ```

2. **Position yourself** in front of the camera with good lighting

3. **Use gestures above the green threshold line** for navigation

4. **Control your presentation**:
   - Hold your hand above the green line for gesture recognition
   - Use thumbs up/pinky gestures to navigate slides
   - Use index finger to draw on slides
   - Use three fingers to erase annotations

5. **Exit**: Press 'q' to quit the application

## 🎨 How It Works

- **Hand Detection**: Uses MediaPipe and CVZone for accurate hand landmark detection
- **Gesture Recognition**: Analyzes finger positions to determine gestures
- **Slide Management**: Automatically loads and displays images from the Presentation folder
- **Annotation System**: Tracks finger movements to create drawings on slides
- **Visual Feedback**: Shows live camera feed with gesture indicators

## 📸 Screenshots

The application displays:
- Main presentation window with current slide
- Small camera preview showing your hand gestures
- Green threshold line for gesture activation
- Real-time annotations and pointer feedback

## 🔧 Configuration

You can modify these parameters in `final.py`:
- `gestureThreshold`: Height threshold for gesture recognition (default: 300)
- `width, height`: Camera resolution (default: 1280x720)
- `delay`: Gesture delay to prevent accidental triggers (default: 30)

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 👨‍💻 Author

**ngmodz** - [GitHub Profile](https://github.com/ngmodz)

## 🙏 Acknowledgments

- CVZone library for hand detection
- OpenCV for computer vision capabilities
- MediaPipe for hand landmark detection

---

*Made with ❤️ for seamless presentation control*