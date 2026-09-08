# 🏋️ Real-Time Voice & Video AI Gym Coach

An AI-powered real-time fitness coach built with **Python, MediaPipe, OpenCV, Streamlit, and Groq AI**. The application uses computer vision and pose estimation to analyze exercises, count repetitions, detect incorrect form, and provide real-time AI voice feedback through a webcam.

---

## 🚀 Live Demo

👉 **AI Real-time GYM Coach — by Vikas Yadav**

**Live demo:** Coming soon — this project will be deployed from the `vikas32210` GitHub repository.

> Allow webcam access in your browser to use real-time exercise tracking.

---

## ✨ Features

- 🎥 Real-time webcam exercise tracking
- 🧍 Real-time human pose estimation
- 🦴 33-point body landmark detection
- 🔢 Automatic repetition counting
- 📐 Joint-angle and movement analysis
- ⚠️ Exercise form and posture detection
- 🤖 AI-powered workout feedback using Groq
- 🔊 AI voice coaching using gTTS
- 🏋️ Multiple exercise support
- 📊 Live workout metrics
- 🌐 Browser-based real-time video streaming
- 🎨 Interactive Streamlit interface

---

## 🧠 Supported Exercises

The application currently supports five exercises:

1. 🏋️ Squats
2. 💪 Push-ups
3. 💪 Biceps Curls (Dumbbell)
4. 🏋️ Shoulder Press
5. 🦵 Lunges

---

## 🛠️ Tech Stack

### 🖥️ Frontend / UI

- Streamlit
- Streamlit WebRTC

### 👁️ Computer Vision

- MediaPipe
- OpenCV
- NumPy

### 🤖 AI

- Groq API

### 🔊 Voice

- gTTS (Google Text-to-Speech)

### ⚙️ Backend / Utilities

- Python
- Pandas
- python-dotenv

---

## 📂 Project Structure

```text
RealTime-Voice-Video-AI-Gym-Coach/

│
├── core/
│   └── base_exercise.py
│
├── detectors/
│   ├── squat.py
│   ├── pushup.py
│   ├── biceps_curl.py
│   ├── shoulder_press.py
│   └── lunges.py
│
├── services/
│   ├── auth/
│   ├── coaching/
│   ├── config/
│   ├── persistence/
│   ├── state/
│   ├── tracking/
│   ├── ui/
│   └── vision/
│
├── static/
│   └── style.css
│
├── ml_models/
│   └── pose_landmarker_full.task
│
├── main.py
├── requirements.txt
├── packages.txt
├── data.db
├── runtime.txt
├── .gitignore
└── README.md
```

---

## ⚙️ Installation

### 1. Clone the Repository

```bash
git clone https://github.com/vikas32210/RealTime-Voice-Video-AI-Gym-Coach.git
cd RealTime-Voice-Video-AI-Gym-Coach
```

### 2. Create a Virtual Environment

#### Windows

```bash
python -m venv .venv
.venv\Scripts\activate
```

#### macOS / Linux

```bash
python3 -m venv .venv
source .venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

---

## 🔐 API Configuration

Create a `.env` file in the project root:

```env
GROQ_API_KEY=your_groq_api_key
```

For deployment, configure the required API credentials using the platform's secret management system.

> Never commit API keys or `.env` files to GitHub.

---

## ▶️ Run Locally

Start the application using:

```bash
streamlit run main.py
```

The application will open in your browser.

---

## 🧠 How It Works

The application processes webcam video in real time through the following pipeline:

1. Webcam captures the user's movement.
2. Streamlit WebRTC streams the video frames.
3. OpenCV processes each frame.
4. MediaPipe detects **33 human body landmarks**.
5. Exercise-specific detectors analyze body movement.
6. Joint angles and posture are calculated.
7. Repetitions are counted automatically.
8. Incorrect exercise form is detected.
9. Groq generates contextual AI coaching feedback.
10. gTTS converts the feedback into voice.
11. Results are displayed through the live video interface.

---

## 🔥 AI Processing Pipeline

```text
Webcam Feed
      ↓
Streamlit WebRTC
      ↓
OpenCV Frame Processing
      ↓
MediaPipe Pose Estimation
      ↓
33 Body Landmarks
      ↓
Exercise Detection
      ↓
Joint Angle & Movement Analysis
      ↓
Rep Counting + Form Detection
      ↓
Groq AI Feedback
      ↓
gTTS Voice Feedback
      ↓
Live Video Output
```

---

## 💡 AI / ML Concepts Used

- Human Pose Estimation
- Real-Time Computer Vision
- Human Landmark Detection
- Motion Tracking
- Joint Angle Calculation
- Exercise Movement Analysis
- Repetition Counting
- Exercise Form Detection
- Generative AI
- AI Voice Feedback
- Real-Time Video Processing

---

## 👨‍💻 Author

### Vikas Yadav

🔗 **GitHub:** https://github.com/vikas32210

---

## ⭐ Project

If you find this project useful, consider giving it a ⭐ on GitHub.
