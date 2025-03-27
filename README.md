# 🚀 Weapon Detection using YOLOv8  

This project implements **real-time weapon detection** using the **YOLOv8** object detection model. It detects weapons in images and live video streams.  

---

## 📌 Project Summary  
Here’s a structured summary of all the steps taken for weapon detection using YOLO:  

### **1️⃣ Setting Up the Environment**  
✅ Installed required dependencies (`ultralytics`, `opencv-python`)  
✅ Used **Google Colab / Jupyter Notebook** to run the project  

### **2️⃣ Downloading the Dataset**  
✅ Used **Roboflow API** to download a **weapon detection dataset**  
✅ Verified that the dataset contained **annotated images** for training  

### **3️⃣ Training the YOLO Model**  
✅ Selected **YOLOv8** as the model architecture  
✅ Trained a **custom YOLOv8 model** (`best.pt`) using the **Roboflow dataset**  
✅ Verified **training logs, validation metrics, and loss curves**  

### **4️⃣ Running Live Weapon Detection**  
✅ Loaded the **trained YOLO model** (`best.pt`) for inference  
✅ Opened **live webcam feed** using **OpenCV**  
✅ Applied **real-time object detection** on video frames  
✅ Drawn **bounding boxes** around detected weapons  

### **5️⃣ Improving Detection & Fixing Errors**  
✅ Fixed **webcam errors** (`cv2.VideoCapture(0)` issues)  
✅ Used `cv2.imshow()` for **real-time frame display**  
✅ Ensured **proper release of webcam** (`cap.release()` & `cv2.destroyAllWindows()`)  
✅ **Increased detection accuracy** by setting a **confidence threshold** (`> 0.5`)  

---

## ✅ Project Status  
✔️ **Working Real-Time Weapon Detection Model** 🚀  

🔹 **Next Steps:**  
- Improve dataset quality  
- Train for more epochs  
- Test in real-world environments  

---

## 📂 Files  
- **`weapon_detection.ipynb`** → Jupyter Notebook with the full implementation  
- **`best.pt`** → Trained YOLOv8 model (not included due to size)  

---

## 🛠 Installation & Setup  

### **🔹 Install Dependencies**  
```sh
pip install ultralytics opencv-python roboflow
