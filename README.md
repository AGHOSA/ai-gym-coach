# AI Gym Coach 🏋️‍♂️

AI Gym Coach is a real-time AI-powered fitness assistant that uses computer vision and generative AI to analyze workout movements, count repetitions, detect form issues, and provide personalized coaching feedback.

## 🚀 Features

- Real-time webcam-based exercise analysis
- Human pose estimation using MediaPipe
- Automatic repetition counting
- Exercise form and posture analysis
- Real-time coaching feedback
- AI-generated feedback using Groq and GPT-OSS 120B
- Voice feedback using Google Text-to-Speech
- Workout sets and repetition tracking
- Local workout history using SQLite
- Streamlit-based interactive web interface

## 🏋️ Supported Exercises

The application currently supports:

- Squats
- Push-ups
- Biceps Curls
- Shoulder Press
- Lunges

## 🧠 How It Works

The system follows this pipeline:

Webcam
→ MediaPipe Pose Landmarker
→ Body Landmark Detection
→ Exercise-Specific Analysis
→ Rep & Form Detection
→ AI Coaching
→ Voice Feedback

The exercise detectors analyze body landmark positions and joint angles to identify movement patterns, repetition states, and common form issues.

## 🛠️ Technologies Used

- Python
- Streamlit
- Streamlit-WebRTC
- MediaPipe
- OpenCV
- NumPy
- Pandas
- Groq API
- GPT-OSS 120B
- Google Text-to-Speech (gTTS)
- SQLite

## 📂 Project Structure

```text
ai-gym-coach/
│
├── LandingPage/
│   ├── index.html
│   └── style.css
│
├── Main App/
│   ├── main.py
│   ├── requirements.txt
│   ├── packages.txt
│   │
│   ├── core/
│   ├── detectors/
│   ├── ml_models/
│   └── services/
│       ├── auth/
│       ├── coaching/
│       ├── config/
│       ├── persistence/
│       ├── state/
│       ├── tracking/
│       ├── ui/
│       └── vision/
│
└── README.md
