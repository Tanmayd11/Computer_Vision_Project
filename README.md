
# 🧠 Feature Detection using Classical Computer Vision Techniques

## 📁 Project Overview

This project demonstrates the implementation of **three classical computer vision algorithms** using OpenCV in Python. These techniques are used in areas such as object detection, motion tracking, and image registration.

The implemented algorithms are:

- **SIFT (Scale-Invariant Feature Transform)**
- **Harris Corner Detector**
- **Shi-Tomasi Corner Detector**

Each algorithm is applied on real-world images, and the visual outputs are generated to show matched keypoints or detected corners.

---

## ✅ Implemented Algorithms

### 🔹 1. SIFT – Scale-Invariant Feature Transform

**Purpose:**  
To detect and match robust keypoints between two images that may vary in scale, rotation, or lighting.

**Steps:**
- Detect keypoints in both images.
- Generate feature descriptors.
- Match descriptors using BFMatcher and apply Lowe’s ratio test.

**Images Used:**  
- `200.jpg`  
- `500.jpg`

**Output:**  
Matched keypoints are shown with lines connecting corresponding points across both images.

---

### 🔹 2. Harris Corner Detector

**Purpose:**  
To detect corners in an image by analyzing changes in pixel intensity.

**Steps:**
- Convert image to grayscale.
- Calculate gradient changes.
- Use the Harris matrix to identify corner strength.
- Mark corners exceeding a defined threshold.

**Image Used:**  
- `cube.jpg`

**Output:**  
Corners are marked with red circles.

---

### 🔹 3. Shi-Tomasi Corner Detector

**Purpose:**  
An enhanced version of Harris Corner Detector selecting high-quality corners.

**Steps:**
- Convert image to grayscale.
- Apply `cv2.goodFeaturesToTrack` to get best corners.
- Mark selected corners on the image.

**Image Used:**  
- `cube.jpg`

**Output:**  
Corners are marked with green circles.

---


## 📦 Requirements

- Python 3.x
- OpenCV (`opencv-python`, `opencv-contrib-python`)
- NumPy
- Matplotlib

---

## 🖼️ Sample Outputs

Each algorithm generates a visual output showing the detected features or matches between two images. The matches or corners are highlighted using colored lines or circles for easy interpretation.

---

## 📚 License

This project is for educational use only. Algorithms like SIFT and SURF may require licensing for commercial applications.

---

## 👨‍🎓 Author

**Name:** Tanmay Dhobale  
**Roll No:** A4_63  
**Institution:** Shri Ramdeobaba College of Engineering and Management
