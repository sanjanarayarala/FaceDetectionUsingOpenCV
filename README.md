# Face Detection using OpenCV  

### Overview  
This project implements **real-time face detection** using **OpenCV's Haar Cascade Classifier**. The program detects faces in both images and live webcam feed, drawing bounding boxes around detected faces.  

### Features  
✔ **Detect faces in static images**  
✔ **Real-time face detection** using webcam  
✔ **Bounding box visualization** with OpenCV  
✔ **Uses Haar Cascade Classifier for face detection**  

### Technologies Used  
- **Python**  
- **OpenCV** – Image processing & face detection  
- **NumPy** – Array manipulation  
- **Matplotlib** – Image visualization  

---

## Project Structure  
```
📂 FaceDetection-OpenCV
 ┣ 📜 face_detection.py
 ┣ 📜 haarcascade_frontalface_default.xml
 ┣ 📜 group.jpg
 ┣ 📜 README.md
```
- `face_detection.py` – Main script for image & real-time face detection  
- `haarcascade_frontalface_default.xml` – Haar cascade model for face detection  
- `group.jpg` – Sample image for testing  

---

## Installation & Setup  

### 1. Install Dependencies  
Ensure you have Python installed along with the required libraries. Run:  
```bash
pip install opencv-python numpy matplotlib
```

### 2. Clone the Repository  
```bash
git clone https://github.com/sanjanarayarala/FaceDetection-OpenCV.git
cd FaceDetection-OpenCV
```

### 3. Run Face Detection on an Image  
Place an image (`group.jpg`) in the project folder and execute:  
```bash
python face_detection.py
```

### 4. Run Real-time Face Detection  
Activate the webcam and detect faces in real time:  
```bash
python face_detection.py --mode live
```

---

## How It Works  
###  **Face Detection in an Image**  
1. Read an image using `cv2.imread()`  
2. Convert BGR to RGB using `cv2.cvtColor()`  
3. Load the **Haar Cascade Classifier** (`haarcascade_frontalface_default.xml`)  
4. Detect faces using `detectMultiScale()`  
5. Draw bounding boxes around detected faces  
6. Display the image using `matplotlib`  

### **Real-time Face Detection**  
1. Capture frames from webcam using `cv2.VideoCapture()`  
2. Convert each frame from BGR to RGB  
3. Detect faces & draw rectangles around them  
4. Display frames in a window  
5. Exit the program when 'q' is pressed  


---

## Future Enhancements  
- Implement **DNN-based** face detection for better accuracy  
- Optimize performance using **multi-threading**  
- Add **face recognition** using deep learning  

---


Let me know if you want to customize it further! 🚀🎯
