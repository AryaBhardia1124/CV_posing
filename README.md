# CV_posing

A real-time pose detection application using computer vision and MediaPipe for human pose estimation.

## 🎯 Overview

CV_posing is a Python application that captures video from your webcam and detects human poses in real-time. It uses MediaPipe's pose detection model to identify key body landmarks and displays them with visual overlays.

## ✨ Features

- **Real-time pose detection** from webcam feed
- **33 body landmarks** detection (MediaPipe Pose model)
- **Visual pose connections** showing skeletal structure
- **Landmark highlighting** with blue circles
- **Mirrored display** for intuitive interaction
- **Easy exit** with 'q' key

## 🚀 Installation

### Prerequisites
- Python 3.7 or higher
- Webcam access

### Setup
1. Clone the repository:
```bash
git clone https://github.com/yourusername/CV_posing.git
cd CV_posing
```

2. Install required dependencies:
```bash
pip install -r requirements.txt
```

## 📦 Dependencies

- **OpenCV** (4.10.0.84) - Computer vision library for video capture and image processing
- **MediaPipe** (0.10.14) - Google's ML framework for pose detection

## 🎮 Usage

1. Run the application:
```bash
python pose.py
```

2. The application will:
   - Open your webcam
   - Display the video feed with pose detection
   - Show body landmarks as blue circles
   - Draw connections between landmarks

3. To exit the application, press the **'q'** key

## 🔧 How It Works

The application uses MediaPipe's pre-trained pose detection model to:
1. Capture frames from your webcam
2. Convert BGR to RGB color space (MediaPipe requirement)
3. Process each frame through the pose detection model
4. Extract 33 body landmarks (nose, shoulders, elbows, wrists, hips, knees, ankles, etc.)
5. Draw the landmarks and connections on the video feed
6. Display the processed video in real-time

## 📊 Pose Landmarks

MediaPipe detects 33 key points on the human body:
- **Face**: nose, eyes, ears
- **Upper body**: shoulders, elbows, wrists
- **Lower body**: hips, knees, ankles
- **Hands**: finger joints
- **Feet**: toe joints

## 🛠️ Customization

You can modify the application by:
- Changing landmark colors (modify the `cv2.circle` color parameter)
- Adjusting landmark size (modify the radius parameter)
- Adding pose classification logic
- Implementing pose tracking across frames
- Adding pose analysis and feedback

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 🙏 Acknowledgments

- [MediaPipe](https://mediapipe.dev/) - For the pose detection model
- [OpenCV](https://opencv.org/) - For computer vision capabilities

## 📞 Support

If you encounter any issues or have questions, please open an issue on GitHub.

---

**Note**: Make sure your webcam is accessible and you have proper lighting for optimal pose detection results.
