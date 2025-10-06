
## **AI Drone | Autonomous Pigeon Repelling with CNN & OpenCV 🐦🤖**




## <img width="40" height="30" alt="Image" src="https://github.com/user-attachments/assets/567d1706-facf-437a-aaca-9f82ccbe51dd" /> Watch the video [here](https://private-user-images.githubusercontent.com/107938584/245761996-a852af70-bcc8-4bc4-b4ee-435e4684a480.mp4?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NTk3NzAzNjYsIm5iZiI6MTc1OTc3MDA2NiwicGF0aCI6Ii8xMDc5Mzg1ODQvMjQ1NzYxOTk2LWE4NTJhZjcwLWJjYzgtNGJjNC1iNGVlLTQzNWU0Njg0YTQ4MC5tcDQ_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjUxMDA2JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI1MTAwNlQxNzAxMDZaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT1mODFmMzkxMzU4ZjQwOGY2NWVjNTA4ZjBiNjJhODA5MmY4ZGZmMjQ0MmFjODJlNTFjZDEwNGYzM2EyN2E0ODQyJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.f2OOFOfpCpHRjfgLuQS6txGr6Jr01ywwHruTxdkEFy0)

https://github.com/Dor12k/Project-Expel-Pigeons-with-AI-Drone/assets/107938584/a852af70-bcc8-4bc4-b4ee-435e4684a480


## System Architecture:

![Image](https://github.com/user-attachments/assets/549354ab-4cf3-4417-9a6c-39c47bb3046e)
Visual representation of modules and data flow: Movement Detection, Object Detection, Object Tracking, AI Model.

<br>

## **Repel Pigeons with AI Drone** 

In this project, we implement algorithms for **Movement Detection**, **Object Detection**, and **Object Tracking**. <br>
Our system recognizes movement in video frames, detects objects, and tracks them in real-time using a camera. <br>
We utilize the **ResNet50** model with **Transfer Learning** techniques on the **CIFAR-10** dataset, achieving an **accuracy of 95%**.

<br>

### Project Overview

**Part 1 - Deep Learning:** <br>
The first phase of this project focuses on **Deep Learning**, specifically **Convolutional Neural Networks** and related topics such as **Overfitting**, **Transfer Learning** (including **Feature Extraction** and **Fine Tuning**), and importing datasets from binary files.


**Part 2 - Computer Vision:** <br>
The second phase involves **Computer Vision**, leveraging libraries such as **OpenCV**, **NumPy**, and **h5py**.

### Model Selection
At the beginning of the project, we experimented with various models and techniques to determine the best fit for recognizing birds. We found that **ResNet50** combined with **Transfer Learning** and **Fine Tuning** produced the highest accuracy of 95% on the **CIFAR-10** dataset.


### Application Functionality
After establishing our model, we developed the application, which operates in two states: **Detection** and **Tracking**. 
Instead of applying the ResNet50 model's predictions for every frame, we detect the object only once at the beginning and then track it throughout the video. For example, processing 2000 frames can significantly reduce computational load, resulting in running the model just once instead of 2000 times. Additionally, we initiate object detection only upon recognizing movement in the frame, optimizing performance during static conditions.

The detection process begins with recognizing movement, after which we isolate the suspicious portion of the frame and send it to the model for prediction. Once the object is detected, we commence tracking. After the tracking phase, the application resumes object detection. We log all detection events with timestamps, displaying this information on the screen, while also saving frames with detection events in a designated folder alongside a text file documenting all occurrences.

### Drone Integration
The system also features a drone mode, which automatically sends the drone to patrol whenever a bird is detected, aiming to expel it. We developed a software development kit (SDK) that allows remote control of the drone via keyboard. The SDK includes a radar display that synchronizes with the drone's location and distance during flight, along with important information such as speed, distance, camera capture capabilities, built-in tracks, detection, and tracking metrics.
User Interface

The application consists of a window divided into six screens:

  1. **Main Frame:** Displays the live camera feed. <br>
  2. **Information Frame:** Contains detection event summaries and application details. <br>
  3. **Tracking Frame:** Shows the object’s coordinates, confidence score, prediction time, and frames per second (FPS). <br>
  4. **Drone Camera Frame:** Displays the drone's camera feed along with its speed, angle, and battery status. <br>
  5. **Scores Frame:** Lists the scores for each detected label. <br>
  6. **Drone Radar:** Synchronizes with the drone's movements and distance. <br>

The application utilizes **TensorFlow** with **Keras** in **Python**.
