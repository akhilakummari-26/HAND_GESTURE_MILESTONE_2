# ✋ Gesture Recognition Interface – Milestone 2

## 📌 Project Overview
The **Gesture Recognition Interface** is a real-time computer vision application that detects hand gestures using a webcam. The system is built using **Streamlit, OpenCV, and MediaPipe** to track hand landmarks and recognize gestures based on the distance between the thumb and index finger.

The application provides a **live visual interface** where users can see detected gestures, measure finger distance, and observe gesture states dynamically. This milestone expands on basic hand detection by introducing **gesture classification logic and distance measurement**.

This system forms a foundation for **gesture-controlled applications**, including volume control, smart interfaces, gaming, and touchless interaction systems.

---

# 🎯 Objectives
- Detect hands in real-time using a webcam
- Track **hand landmarks** using MediaPipe
- Measure distance between **thumb and index finger**
- Classify gestures based on finger distance
- Display gesture states in a **Streamlit interface**
- Visualize gesture metrics using **cards and progress bars**

---

# 🛠️ Technologies Used

| Technology | Purpose |
|------------|--------|
| Python | Core programming language |
| Streamlit | Interactive web application |
| OpenCV | Video capture and frame processing |
| MediaPipe | Hand tracking and landmark detection |
| HTML/CSS | User interface styling |

---

# 📂 Project Structure

```
HAND_GESTURE_MILESTONE2
│
├── milestone2.py
├── README.md

```

---

# ⚙️ Installation

## 1️⃣ Clone the Repository

```bash
git clone https://github.com/akhilakummari-26/HAND_GESTURE_MILESTONE_2.git

```

---

## 2️⃣ Install Dependencies


 Install the below libraries

```bash
pip install streamlit opencv-python mediapipe
```

---

# ▶️ Running the Application

Run the Streamlit application using:

```bash
streamlit run milestone2.py
```

The application will open in your browser at:

```
http://localhost:8501
```

---

# 🖥️ Application Interface

The interface is divided into two sections.

### Left Panel
- Displays **live webcam feed**
- Shows **hand landmark detection**
- Visualizes finger distance and gesture label

### Right Panel

#### 📏 Distance Measurement
Displays:
- Distance between **thumb and index finger**
- Progress bar representing distance scale

#### ✋ Gesture States
Shows:
- Open Hand
- Pinch
- Closed

The current detected gesture is highlighted dynamically.

---

# 🧠 Gesture Recognition Logic

The system measures the **distance between two landmarks**:

- Thumb Tip (Landmark 4)
- Index Finger Tip (Landmark 8)

Using the formula:

```
distance = √((x2 - x1)² + (y2 - y1)²)
```

The distance determines the gesture type.

---

# ✋ Gesture Classification

| Gesture | Distance |
|-------|--------|
| Closed | Distance < 30 |
| Pinch | 30 ≤ Distance < 80 |
| Open Hand | Distance ≥ 80 |

---

# 🎮 Controls

| Button | Function |
|------|------|
| ▶ Start | Activates webcam |
| ⏸ Pause | Stops camera feed |
| ⚙ Settings | Reserved for future configuration |

---

# 📊 Features

- Real-time webcam gesture detection
- Thumb–index finger distance measurement
- Gesture classification
- Dynamic UI with progress bars and cards
- Live gesture visualization
- Smooth webcam streaming

---

# 🚀 Future Improvements

Future milestones may include:

- 🔊 **Gesture-based volume control**
- 🤖 **Machine learning gesture classification**
- 📱 **Smart touchless interfaces**
- 🎮 **Gesture control for games**
- 📊 **Improved gesture accuracy**

---

# 📚 Applications

Gesture recognition technology can be used in:

- Smart home control systems
- Touchless interfaces
- Gaming and AR/VR systems
- Assistive technology
- Human-computer interaction
- Medical environments

---

# 👩‍💻 Author

**Akhila Kummari**

---

# 📜 License

This project is licensed under the MIT License.
