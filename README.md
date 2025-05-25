# 🚨 SleepGuard - Web-based Driver Drowsiness Detection

SleepGuard is a lightweight, browser-based driver drowsiness detection system built using **Next.js**, **React Webcam**, and **face-api.js**. Designed with simplicity and safety in mind, it simulates an emergency response when signs of driver fatigue are detected — even in the absence of internet (offline logic simulated via UI/local triggers).

> ⚡ Built for demos, safety awareness, and real-world prototypes of intelligent transport safety systems.

---

## 🌟 Features

- 🔍 **Live Drowsiness Detection** using Eye Aspect Ratio (EAR)
- 📷 **Webcam Access** for real-time monitoring
- 📍 **GPS Location Capture** using HTML5 Geolocation API
- 🚨 **Simulated Emergency Alert** via modal & API call
- 📊 Real-time status logs for testing & debugging
- ☁️ Deployed on **Vercel** for instant access

---

## 📸 How It Works

SleepGuard uses your webcam and face landmarks to calculate the Eye Aspect Ratio (EAR). When the EAR drops below a threshold (indicating closed eyes) for more than 3 seconds, the app:
- Triggers an on-screen alert
- Logs the event time and your last known location
- (Optional: can be extended to notify emergency contacts)

---

## 🛠️ Tech Stack

| Purpose              | Tech Used                    |
|----------------------|------------------------------|
| Frontend Framework   | Next.js (React + TypeScript) |
| Camera Access        | `react-webcam`               |
| Face & Eye Detection | `face-api.js`                |
| Location Detection   | `navigator.geolocation` API  |
| Alert System         | Modal + API simulation       |
| Deployment           | Vercel                       |

---

## 🚀 Getting Started

### Prerequisites

- Node.js 18+
- Git

### Installation

```bash
git clone https://github.com/your-username/sleepguard.git
cd sleepguard
npm install
npm run dev
