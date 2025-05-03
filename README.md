## Face_Recognition
#### 🧠 Face Recognition System using OpenCV.
This project implements a real-time face recognition system using a webcam feed. It utilizes OpenCV's Haar Cascade classifier for face detection and Logistic Regression for face recognition. The system supports face registration and live recognition by comparing against stored facial encodings.


#### 📁 Project Structure
The core logic is organized into four main functions:
1. save_face(name, number_of_faces_to_capture) => capture a person's face and save it in provided 'name' directory inside faces directory.
2. save_faces_to_csv() => saves all faces as csv in 'generated_dataset' directory and deletes face data. (concats with previous dataset if exist)
3. model_fit() => train model with LinearSVC
4. predict() => recognise face on the camera

#### 🛠️ Requirements
1. Python 3.x
2. OpenCV
3. NumPy

#### 📦 How to Use
1. Add a new face using save_face() function with name as first argument and number of faces as second argument.
2. Run the save_faces_to_csv() function to register a new person.
3. Train the model using model_fit().
##### Start recognition
4. Call predict() to begin real-time face recognition using the webcam.

#### 📌 Notes
1. Ensure that the haarcascade_frontalface_default.xml file is present in your working directory or adjust the path accordingly in the code.

#### ✅ Features
1. Real-time face detection and recognition via webcam.
2. Lightweight model — no GPU or deep learning model required.
3. Easily extendable by adding new images in dataset.

#### 🔒 Limitations
1. This works well for frontal faces but may perform poorly under significant lighting or angle variations.

#### ✅ Conclusion
In this project, we successfully implemented a real-time face recognition system using OpenCV's LBPH (Local Binary Patterns Histogram) algorithm. We built a pipeline to detect faces from a live webcam feed, label them using a custom dataset, and recognize them in real time. The system is lightweight and does not require a deep learning model or GPU, making it suitable for quick prototyping and educational purposes.

