# Eye-Controlled Mouse

Eye-Controlled Mouse is an innovative project that allows users to control the mouse cursor and perform clicks using just their eye movements. Utilizing real-time facial landmark detection through **OpenCV** and **Mediapipe**, this hands-free interaction offers a glimpse into advanced human-computer interaction, particularly useful for accessibility purposes.

---

## Key Features:
- **Real-Time Eye Tracking**: Detects and tracks key facial landmarks, specifically focusing on the eyes, to interpret gaze direction.
- **Cursor Movement**: Maps eye positions to screen coordinates, enabling mouse movement across the screen.
- **Blink Detection for Clicks**: Monitors blinking patterns to trigger mouse clicks when a significant eye closure is detected.
- **Accurate Facial Landmark Recognition**: Powered by **Mediapipe's Face Mesh**, which detects 468 key landmarks on the face with precision.

---

## How It Works:

1. **Camera Input**: The webcam captures the video feed, which is then processed frame-by-frame.
2. **Face Mesh Processing**: Mediapipe’s Face Mesh model extracts 468 landmarks from the face, refining key landmarks near the eyes for gaze tracking.
3. **Cursor Mapping**: The landmark coordinates are scaled and mapped onto the screen dimensions to move the mouse cursor accordingly.
4. **Blink Detection**: The distance between two specific eye landmarks is monitored. When the distance falls below a threshold (indicating a blink), a mouse click is triggered.
   
---

## Installation

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/TejasUpadhyayy/Eye-controlled-Mouse.git
   ```

2. **Install Dependencies:**

   Install the required Python libraries:

   ```bash
   pip install opencv-python mediapipe pyautogui
   ```

3. **Run the Script:**

   Ensure your webcam is connected, then execute:

   ```bash
   python eye_controlled_mouse.py
   ```

---

## Requirements:
- **Python 3.x**
- **OpenCV**: For capturing and processing the video feed.
- **Mediapipe**: To detect and track facial landmarks.
- **PyAutoGUI**: For controlling mouse actions (movement and clicks).

---

## Customization:
- **Threshold Adjustment**: The blink detection threshold (`0.004` in the script) can be fine-tuned for different lighting conditions or camera setups to avoid false positives.
- **Screen Resolution**: The script automatically scales the cursor movement based on screen resolution, but this can be adjusted in the code for custom resolutions.

---

## Applications:
- **Accessibility**: Provides hands-free control for individuals with mobility impairments.
- **Human-Computer Interaction**: Offers a novel interface for interacting with computers through gaze control.
- **Eye-Tracking Research**: Can serve as a foundation for more advanced gaze-tracking and eye-movement analytics systems.

---

## Future Enhancements:
- **Right-Click Support**: Introducing right-click functionality based on longer blinks or other facial cues.
- **Multi-User Calibration**: Implementing user-specific calibration for enhanced precision.
- **Eye Gesture Recognition**: Expanding the system to recognize complex eye gestures for more detailed control.

---

## Contact Me:

For any queries, suggestions, or collaboration opportunities, feel free to reach out:

- **Email**: [tejas.initiate@gmail.com]
- **LinkedIn**: [Your LinkedIn Profile](#)
