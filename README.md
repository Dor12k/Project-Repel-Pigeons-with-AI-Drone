
## **AI Drone | Autonomous Pigeon Repelling with CNN & OpenCV 🐦🤖**


An AI-powered drone system using **Deep Learning** and **Computer Vision** to implement **Object Detection**, <br>**Object Tracking**, and 
**Autonomous Flight** for repelling pigeons in real time and reducing garden pest damage.  
Built with **TensorFlow**, **OpenCV**, **NumPy**, and **Python**, featuring GPS simulation and motion-triggered detection.  <br><br>
Demonstrates hands-on experience in **AI model training**, **real-time systems**, and **autonomous robotics**.



## <img width="40" height="30" alt="Image" src="https://github.com/user-attachments/assets/567d1706-facf-437a-aaca-9f82ccbe51dd" /> Watch the video [here](https://private-user-images.githubusercontent.com/107938584/245761996-a852af70-bcc8-4bc4-b4ee-435e4684a480.mp4?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NTk3NzAzNjYsIm5iZiI6MTc1OTc3MDA2NiwicGF0aCI6Ii8xMDc5Mzg1ODQvMjQ1NzYxOTk2LWE4NTJhZjcwLWJjYzgtNGJjNC1iNGVlLTQzNWU0Njg0YTQ4MC5tcDQ_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjUxMDA2JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI1MTAwNlQxNzAxMDZaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT1mODFmMzkxMzU4ZjQwOGY2NWVjNTA4ZjBiNjJhODA5MmY4ZGZmMjQ0MmFjODJlNTFjZDEwNGYzM2EyN2E0ODQyJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.f2OOFOfpCpHRjfgLuQS6txGr6Jr01ywwHruTxdkEFy0)

https://github.com/Dor12k/Project-Expel-Pigeons-with-AI-Drone/assets/107938584/a852af70-bcc8-4bc4-b4ee-435e4684a480

---

## 🧩 System Architecture

![System Graph](https://github.com/user-attachments/assets/549354ab-4cf3-4417-9a6c-39c47bb3046e)

> The architecture shows how deep learning, computer vision, and autonomous navigation modules interact in real time.

---

## 🌿 Overview

An **AI-powered autonomous drone system** that uses **deep learning** and **computer vision** to detect, track, and repel pigeons in real time.  
The system combines movement detection, object tracking, and autonomous navigation to create a smart pest control solution powered by artificial intelligence.

This project integrates **Deep Learning, Computer Vision, and Robotics** to build an end-to-end intelligent drone system.  
A stationary camera monitors the garden and detects pigeons using a trained CNN model. Once detected, a drone autonomously navigates toward the target to repel it — minimizing human intervention and protecting crops.






## ⚙️ Project Workflow

### **1. Model Training (Deep Learning Phase)**
- Built and trained **CNN models** (ResNet50, VGG16, AlexNet) on the **CIFAR-10** dataset.  
- Applied **Transfer Learning** (Feature Extraction & Fine-Tuning) and **Data Augmentation**.  
- Controlled **Overfitting** and evaluated models using accuracy/loss graphs and a **confusion matrix**.  
- Selected **ResNet50** as the best-performing model with **95% accuracy** for object recognition.

### **2. Object Detection & Tracking (Computer Vision Phase)**
- Implemented real-time motion detection using **OpenCV** and **NumPy**.  
- Frames are analyzed for motion; only changed regions are passed to the CNN for classification — ensuring efficiency and reduced computational load.  
- The system records each detection with a timestamp and saves relevant frames and logs.

### **3. Autonomous Drone Navigation (AI Robotics Phase)**
- Developed an algorithm for **autonomous flight and object tracking**.  
- Added **GPS simulation** to visualize movement and drone path across the garden.  
- The drone can patrol predefined coordinates and react dynamically to pigeon detection.

---

## 🚀 Key Features

✅ Real-time object detection and tracking  
✅ Deep Learning with Transfer Learning & Fine-Tuning  
✅ Autonomous drone navigation  
✅ GPS simulation and live path visualization  
✅ Data logging and event-based frame saving  

---

## 🧰 Tech Stack

**Programming Language:** Python  
**Deep Learning:** TensorFlow, Keras  
**Computer Vision:** OpenCV, NumPy  
**Data Analysis & Visualization:** Matplotlib, Pandas  
**Performance:** Multithreading (for real-time execution)

---

## 📊 Results

- Achieved **95% classification accuracy** using ResNet50 with Transfer Learning.  
- Generated detailed performance graphs and confusion matrices for analysis.  
- Demonstrated seamless integration between AI-based detection and drone navigation.

---

## 🔮 Future Improvements

- Integrate **YOLOv8** for enhanced real-time detection and faster inference.  
- Add **hardware-based GPS** and drone SDK support (e.g., DJI or ArduPilot).  
- Extend system scalability for multi-drone coordination.

---

## 📁 Repository Structure

📦 AI-Drone-Autonomous-Pigeon-Repelling

┣ 📂 Drone

┣ 📂 Model

┣ 📂 System

┗ 📂 OpenCV (Beta version - early prototypes)

---

## 💡 Summary

This project demonstrates hands-on expertise in **Deep Learning, Computer Vision, and Autonomous Systems**, integrating software intelligence with real-world robotics.  
It highlights practical experience in **AI model development**, **system design**, and **Python engineering** — bridging the gap between **machine learning** and **real-time embedded applications**.

---

