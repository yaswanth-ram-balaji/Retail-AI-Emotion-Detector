# 🛍️ Retail AI – Emotion Detector

**Real-Time Facial Emotion Recognition for Customer Experience**

The **Retail AI-Emotion Detector** is an AI-powered real-time emotion tracking system designed to measure customer satisfaction using live facial expression analysis.
It uses a **DeepFace-based emotion model**, a **Spring Boot backend**, and a **React + Vite frontend** to deliver actionable emotion analytics for retail environments.

---

## 📌 Features

### 🎭 **Real-Time Emotion Detection**

* Detects 7 emotions: **Happy, Sad, Angry, Neutral, Fear, Surprise, Disgust**
* Uses **DeepFace** for high-accuracy emotion classification
* Live webcam feed processing

### 👤 **Customer Journey Tracking**

* Logs **Entry Emotion** and **Exit Emotion**
* Computes **Satisfaction Delta**
* Helps identify positive/negative experiences instantly

### 📊 **Dashboard & Analytics**

* Emotion heatmaps
* Hourly trends
* Emotion distribution (pie/bar charts)
* Satisfaction meter & insights
* Auto recommendations based on patterns

### 🔒 **Privacy & Ethics**

* Optional **Face Blur** feature
* Secure handling of frames and session data

### 🧩 **Modular Architecture**

* **Frontend:** React + TypeScript + TailwindCSS
* **Backend:** Spring Boot REST API
* **AI Layer:** Python FastAPI + DeepFace + OpenCV
* **Database:** MySQL / MongoDB (for emotion logs)

---

## 🏗️ Project Architecture

```
Frontend (React)  →  Backend (Spring Boot)  →  AI Service (Python + DeepFace)
          ↑                     ↓                     ↑
       User UI         API for session/data     Emotion prediction
```

---

## 📁 Project Structure (Simplified)

```
EMOTION-SENSE/
│
├── emotion-backend/
│   └── main.py  # DeepFace emotion analysis API
│
└── emotion-sense-retail-ai/
    ├── src/
    │   ├── components/
    │   ├── pages/
    │   ├── services/
    │   └── utils/
    ├── public/
    ├── package.json
    └── vite.config.ts
```

---

## 🧪 Tech Stack

### **Frontend**

* React + Vite
* TypeScript
* TailwindCSS
* Chart.js / Recharts

### **Backend**

* Spring Boot
* REST APIs
* Tomcat Embedded

### **AI / ML Layer**

* DeepFace
* OpenCV
* FastAPI
* NumPy, PIL

### **Tools**

* VS Code / IntelliJ
* Postman
* Git & GitHub

---

## 🚀 How It Works (Flow)

1. Webcam captures real-time frames
2. Frames sent to Spring Boot backend
3. Backend → Forwards to Python/DeepFace API
4. DeepFace predicts emotion + confidence
5. Backend stores + returns results
6. Frontend updates dashboards live

---

## 📸 Sample Outputs

### ✔️ Detected Emotions

```
Emotion: Happy  
Confidence: 89.5%
```

### ✔️ Entry–Exit Satisfaction Example

| Entry   | Exit  | Result              |
| ------- | ----- | ------------------- |
| Neutral | Happy | Positive Experience |
| Neutral | Angry | Negative Experience |

### ✔️ Heatmap & Trends

* Peak unhappy hours
* Hourly emotion frequency
* Satisfaction ratio

---

## 💡 Insights Generated

* “High unhappy activity at 9 PM — add staff.”
* “Satisfaction improved by 12% this week.”
* “Negative emotion hotspot detected in Zone 3.”

---

## 📌 Setup Instructions

### **AI Backend (Python)**

```bash
cd emotion-backend
pip install -r requirements.txt
uvicorn main:app --reload
```

### **Frontend**

```bash
cd emotion-sense-retail-ai
npm install
npm run dev
```

### **Spring Boot Backend**

```
Run as Maven/Gradle project
```

---

## 🌐 Deployment Link

🔗 **Live App:** [https://emotion-sense-retail-ai.lovable.app](https://emotion-sense-retail-ai.lovable.app)

---

## 📚 References

* DeepFace: [https://github.com/serengil/deepface](https://github.com/serengil/deepface)
* OpenCV: [https://opencv.org](https://opencv.org)
* Vite: [https://vitejs.dev](https://vitejs.dev)
* TailwindCSS: [https://tailwindcss.com](https://tailwindcss.com)

---

## 🏁 Conclusion

This project demonstrates how **AI + Web Technologies** can transform real-time customer experience in retail.
It enables **accurate emotion monitoring**, **satisfaction analytics**, and **data-driven decisions** for business improvement.

