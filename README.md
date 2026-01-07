# 🖐️ Hand Gesture Controlled Mouse using Python & MediaPipe

This project allows you to control your computer mouse using hand gestures captured via a webcam. It uses MediaPipe for real-time hand landmark detection and PyAutoGUI / Pynput to perform mouse actions such as movement, left click, right click, double click, and taking screenshots.

## ✨ Features

- Real-time hand tracking using webcam  
- Mouse movement using index finger  
- Left click, right click, and double click gestures  
- Screenshot capture using hand gesture  
- Works on any screen resolution  

## 🛠️ Tech Stack

- Python 3.x  
- OpenCV  
- MediaPipe  
- PyAutoGUI  
- Pynput  
- NumPy  

## 📂 Project Structure

Hand-Gesture-Controlled-Mouse/  
├── main.py        # Main application (gesture detection & mouse control)  
├── util.py        # Utility functions (angle & distance calculations)  
├── README.md      # Project documentation  
└── my_screenshot_*.png  

## ⚙️ Installation & Setup

1. Clone the repository  
git clone https://github.com/vksoni10/Hand-gesture-controlled-mouse.git 
cd hand-gesture-controlled-mouse  

2. (Optional) Create a virtual environment  
python -m venv venv  
source venv/bin/activate   # Linux / macOS  
venv\Scripts\activate      # Windows  

3. Install required dependencies  
pip install opencv-python mediapipe pyautogui pynput numpy  

## ▶️ How to Run

python main.py  

- Make sure your webcam is connected  
- A window will open showing detected hand landmarks  
- Press `q` to exit the application  

## ✋ Hand Gesture Controls

Index finger open, thumb close → Mouse movement  
Index finger bent → Left click  
Middle finger bent → Right click  
Index + middle finger bent → Double click  
Thumb close to index + bent fingers → Screenshot  

Screenshots are saved automatically as:  
my_screenshot_<random_number>.png  

## 🧠 How It Works

- MediaPipe Hands detects 21 hand landmarks in real time  
- Angles between finger joints are used to detect finger bending  
- Distance between thumb and index finger helps distinguish gestures  
- PyAutoGUI and Pynput simulate mouse actions  

## ⚠️ Notes & Tips

- Use good lighting for better detection accuracy  
- Keep your hand within the camera frame  
- Webcam quality affects tracking performance  
- Run with administrator privileges if mouse control does not work  

## 🚀 Future Improvements

- Smooth cursor movement  
- Scroll gestures  
- Multi-hand support  
- Custom gesture mapping  
- GUI-based settings  

## 👨‍💻 Author

Your Name  
GitHub: https://github.com/your-username  

## ⭐ Support

If you found this project useful, please give it a ⭐ on GitHub!
