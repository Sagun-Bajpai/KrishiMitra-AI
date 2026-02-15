# 🏗 KrishiMitra AI – System Design Document

---

## 1️⃣ System Overview

KrishiMitra AI follows a **microservice-based architecture** where the frontend communicates with a Spring Boot backend, which further interacts with AI services and databases deployed on AWS Cloud.

---

## 2️⃣ High-Level Architecture

Farmer (User)  
⬇  
React Frontend  
⬇  
Spring Boot Backend  
⬇  
AI Microservice (Python ML Model)  
⬇  
MySQL Database  
⬇  
AWS Cloud Infrastructure  

---

## 3️⃣ Workflow Design

### 🌾 Crop Disease Detection Flow

1. Farmer uploads crop image  
2. Frontend sends image to Spring Boot API  
3. Backend forwards image to AI model service  
4. AI model predicts disease type  
5. Suggested remedy fetched from database  
6. Result displayed to farmer  

---

### 📊 Mandi Price Prediction Flow

1. Market data collected from APIs  
2. Data stored in MySQL database  
3. ML model performs time-series analysis  
4. Predicted prices displayed on dashboard  

---

## 4️⃣ AI Components

- 🧠 Computer Vision (CNN-based model) for crop disease detection  
- 📈 Time-Series Forecasting Model for mandi price prediction  
- 💬 NLP-based chatbot for farmer queries  

---

## 5️⃣ Technology Stack

- **Frontend:** React.js  
- **Backend:** Java Spring Boot  
- **Database:** MySQL  
- **AI Services:** Python (TensorFlow / Scikit-learn)  
- **Cloud:** AWS (EC2, S3, RDS)  

---

## 6️⃣ Security Design

- 🔐 JWT-based authentication  
- 🔒 Role-based access control  
- 🛡 Secure REST API endpoints  

---

## 7️⃣ Scalability Plan

- ☁ AWS Cloud Deployment  
- ⚙ Microservice-based architecture  
- 📊 Load balancing for high traffic  
- 📦 Future support for mobile app integration
