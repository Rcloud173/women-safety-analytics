# Women Safety Analytics 🚨

## 🔍 Problem Summary

With increasing concerns around women's safety in urban areas, there's an urgent need for smart surveillance systems that can **proactively detect and prevent threats**. Traditional systems react *after* incidents happen. Our solution introduces **real-time analytics** using computer vision and AI to detect **anomalies and SOS gestures**, identify potential dangers, and alert authorities **before harm occurs**.

---

## 🎯 Objective

Develop a real-time video analytics system with the following capabilities:
- Detect people and classify gender
- Analyze gender distribution
- Detect lone women at night
- Detect a woman surrounded by men
- Recognize SOS gestures
- Identify hotspots based on historical alerts

---

## 👥 Target Audience

### End Users:
- **Law enforcement agencies**
- **City surveillance & control rooms**
- **Smart city administrators**
- **Concerned citizens (via alerts or dashboards)**

### Pain Points:
- Delayed response to crimes
- Lack of context in surveillance footage
- Inability to detect early warning signs
- No data-driven city planning for women’s safety

---

## 💡 Proposed Solution

### Project Name: **SheGuardian**

A real-time analytics engine powered by AI and computer vision to proactively identify potential threats and send alerts.

### 🔑 Key Features:
- **Live Person Detection with Gender Classification**
- **Gender Ratio Estimation in a Scene**
- **Nighttime Lone Woman Detection**
- **Surrounded Woman Detection Logic**
- **Gesture-based SOS Recognition (e.g. palm-out hand signal)**
- **Heatmap Generation of High-Risk Zones (Hotspots)**

---

## 🏗️ Architecture & Implementation

### System Diagram:

[Camera Feed] --> [AI Inference Engine]
|
+-------------------+-------------------------+
| | |
[Object Detection] [Gender Classifier] [Gesture Detector]
| | |
[Person Counts] [Lone Woman Detector] [SOS Detection]
| | |
+---------> [Alert System + API] <------------+
|
[Dashboard + Map]

### 🔧 Technologies & Tools:

- **Languages**: Python
- **AI Frameworks**: TensorFlow, PyTorch
- **CV Library**: OpenCV, Mediapipe
- **Models**:
  - YOLOv8 or EfficientDet for object/person detection
  - Custom CNN for gender classification
  - LSTM + Pose Estimation (Mediapipe) for gesture detection
- **Backend**: Flask or FastAPI
- **Database**: PostgreSQL / Firebase (for real-time alerts + logs)
- **Visualization**: Plotly Dash / Streamlit / Leaflet.js (for heatmaps)

---