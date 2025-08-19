# ASANA-AI🧘‍♀
Yoga Pose Detector, Pose Corrector & Meditation Module
📌 Project Overview
Asana AI is a web-based application that helps users detect, learn, and correct yoga poses while also supporting mindfulness through a meditation module.
It combines MediaPipe’s AI-based pose detection with custom logic to provide real-time feedback (including voice guidance) to improve posture accuracy, flexibility, and overall wellness.

✨ Features

🧍 Pose Detector → Identifies yoga poses like Mountain, Goddess, Garland, Plank.

✅ Pose Corrector → Guides and corrects poses like Tree, Chair, Cobra, Warrior, Dog, Shoulderstand.

🎤 Voice Feedback → Announces if the pose is correct or provides live correction (“Straighten your back”, “Lift your arm higher”).

📖 Step-by-Step Instructions → Text + visual guidance for proper alignment.

🧘 Meditation Module → Encourages relaxation and mindfulness.

🌐 Beginner-Friendly UI → Simple navigation, dropdown pose selection, and easy learning flow.

🤖 How Pose Detection Works

Asana AI uses MediaPipe Pose along with rule-based logic and text-to-speech feedback.

Pose Landmark Detection

MediaPipe detects 33 body keypoints (joints like shoulders, elbows, hips, knees, ankles).

Each point has (x, y, z) coordinates + visibility score.

Geometric Analysis

The system calculates angles between joints (e.g., elbow angle, knee bend).

Checks relative positions (e.g., hand above head, foot against thigh).

Pose Comparison

Detected pose is compared with ideal yoga pose data.

If within range → pose is correct.

If not → system identifies misaligned joints.

Voice Feedback System

Uses Web Speech API (TTS) for real-time corrections.

Examples:

✅ “Perfect! Your Tree Pose looks great.”

⚠️ “Straighten your spine.”

⚠️ “Lift your right arm higher.”

Correction Loop

User adjusts posture → system rechecks continuously → confirms when pose is correct.

👉 In short:
MediaPipe finds body landmarks → angles are calculated → compared with yoga pose rules → voice tells you if it’s correct or how to fix it.

🛠️ Tech Stack

Frontend → HTML, CSS, JavaScript

Pose Detection → MediaPipe Pose

Computer Vision → Geometry-based angle calculations

Voice Feedback → Web Speech API (Text-to-Speech)

Hosting → Netlify

📂 Project Structure
AsanaAI/
│── home.html         # Homepage  
│── PoseDetector/     # Yoga pose detection module  
│── PoseCorrector/    # Pose correction module with instructions  
│── meditation/       # Meditation module  
│── assets/           # Images & illustrations  
│── styles/           # CSS files  
│── scripts/          # JavaScript logic (pose + feedback)  

🚀 How to Run Locally

Clone the repository:

git clone https://github.com/yashaswini25-codes/AsanaAI.git


Open home.html in a browser.

Select a module: Pose Detector, Pose Corrector, or Meditation.

Allow camera & audio access for pose detection + voice feedback.

📌 Future Enhancements

🔴 Real-time AI-based classifier for automatic pose recognition.

📊 Personalized progress tracking & yoga routines.

🎧 Guided meditation with audio/visual support.

📱 Mobile-responsive version with improved UI.

📜 License

This project is licensed under the MIT License.




🔥 This is t
