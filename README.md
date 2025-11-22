# Hand Gesture PPT Controller 🖐️

Control your presentations with hand gestures using your webcam! Navigate slides and draw annotations without touching your keyboard.

## Features
- Navigate slides with thumbs up/pinky gestures
- Draw on slides with index finger
- Erase annotations with three fingers
- Real-time hand tracking

## Installation
```bash
git clone https://github.com/ngmodz/hand-gesture-ppt-controller.git
cd hand-gesture-ppt-controller
pip install opencv-python cvzone numpy
```

## Setup
1. Place your presentation images (PNG) in the `Presentation` folder
2. Run: `python final.py`
3. Hold your hand above the green line for gesture control
4. Press 'q' to quit

## Hand Gestures
- 👍 **Thumbs up** → Previous slide
- 🤙 **Pinky up** → Next slide  
- ☝️ **Index finger** → Draw mode
- ✌️ **Two fingers** → Pointer mode
- 🤟 **Three fingers** → Erase

Built with OpenCV and CVZone