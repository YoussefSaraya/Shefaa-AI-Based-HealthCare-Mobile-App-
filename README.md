# 🏥 AI Mobile Healthcare Application

An **AI-powered cross-platform mobile healthcare app** built with **Flutter** and **Firebase**, integrating **state-of-the-art AI models** to deliver accessible, intelligent, and scalable healthcare solutions.

This project was developed as a **Final Year Graduation Project** at **Egypt-Japan University of Science and Technology (E-JUST)**.

---

## 🚀 Features

- **Image Diagnostics**
  - 🦴 **X-ray Fracture Detection** (YOLOv8 + FastAPI backend)
  - 🩹 **Wound Classification** (MobileNetV2, TensorFlow Lite optimized)
  - 🩺 **Skin Disease Diagnosis** (DenseNet-121 trained on HAM10000)

- **Conversational & Mental Health AI**
  - 💬 **Medical Chatbot** (RAG + LLaMA-3, English & Arabic, Pinecone + LangChain)
  - 🧠 **Mental Health Classifier** (Transformer-based, context-aware monitoring)

- **Smart Healthcare Tools**
  - 📅 **Doctor Booking System** (Firebase Realtime Database + Auth)
  - ⏰ **Pill Alarm Reminders** (Local notifications, Firebase sync)
  - 🍽 **Dietary Recommendation System** (Rule-based meal planner with health constraints)

---

## 🏗 Tech Stack

- **Frontend**: Flutter (Dart)
- **Cloud/Database**: Firebase (Auth, Realtime Database, Storage, Notifications)
- **Backend for AI models**: Python FastAPI
- **Machine Learning**:
  - YOLOv8 (Ultralytics, PyTorch) – Fracture detection
  - MobileNetV2 – Wound classification
  -  – Skin disease detection
  - Transformers (LLaMA-3 / BERT) – Mental health analysis
  - LangChain + Pinecone – Retrieval-Augmented Generation chatbot
- **Deployment**: TensorFlow Lite (mobile inference), FastAPI endpoints

---

## 📂 Repository Structure

healthcare-ai-app/
│
├── mobile_app/ # Flutter app
│ ├── lib/ # Main Dart code
│ │ ├── core/ # Shared utils, themes
│ │ ├── features/ # Features (chatbot, diagnosis, booking, diet)
│ │ ├── services/ # Firebase services
│ │ └── widgets/ # Reusable widgets
│ ├── assets/ # Images, icons, fonts
│ └── pubspec.yaml
│
├── firebase/ # Firebase configs & rules
│ ├── firebase_rules/ # Firestore & Storage rules
│ ├── google-services.json # Android config (not committed)
│ └── GoogleService-Info.plist # iOS config (not committed)
│
├── ai_models/ # ML models & training
│ ├── notebooks/ # Colab / Jupyter experiments
│ ├── src/ # Preprocessing, training, inference
│ ├── saved_models/ # Exported weights (TF Lite / PyTorch)
│ └── evaluation/ # Metrics & reports
│
├── docs/ # Documentation
│ ├── architecture.png
│ ├── requirements.md
│ └── user_manual.md
│
└── README.md

yaml

## ⚙️ Setup & Installation

### 1. Clone the repo
```bash
git clone https://github.com/<your-username>/healthcare-ai-app.git
cd healthcare-ai-app
2. Install dependencies
bash
Copy code
cd mobile_app
flutter pub get
3. Configure Firebase
Add google-services.json (Android) in /android/app/.

Add GoogleService-Info.plist (iOS) in /ios/Runner/.

Set up Firebase Auth, Firestore rules, and Realtime Database.

4. Run the app
bash
Copy code
flutter run

🧪 AI Models Usage
X-ray Fracture Detection: Upload radiograph → YOLOv8 detects fractures

Wound Classifier: Upload wound image → MobileNetV2 outputs category

Skin Disease Classifier: Upload skin photo → predicts class

Chatbot: Type query → RAG chatbot retrieves & generates medical response

Diet Planner: Enter profile → Generates 7-day meal plan

Models are trained in ai_models/notebooks/ and deployed via FastAPI endpoints or TensorFlow Lite.

📊 Evaluation (Highlights)
YOLOv8 fracture detection: ~92% accuracy

DenseNet-121 skin disease classification: high F1-scores across classes

Chatbot latency: ~1.2s per query (quantized LLaMA-3)

Real-time Firebase booking & reminders tested under simulated load
Shefaa Thesis


👥 Contributors
Youssef Saraya
Roaa Hatem
Mohamed Hisham
Omar Medhat
Noureen Ayman
Marwa Ahmed
Supervisor: Dr. Reda El Bassiouny

⚠️ Disclaimer
This application is not a substitute for professional medical advice.
All AI outputs are supportive tools and should be used under clinical supervision.

📜 License
MIT License
