
# 🧠 Computer Vision Techniques – Feature Detection & Matching

## 📁 Project Overview

This project implements and visualizes **feature detection and matching techniques** used in computer vision. The following algorithms have been implemented using Python and OpenCV:

- **SIFT (Scale-Invariant Feature Transform)**
- **RANSAC (Random Sample Consensus)**
- **Harris Corner Detector**
- **Shi-Tomasi Corner Detector**

These techniques are foundational in tasks like object detection, image stitching, structure from motion, and panorama creation.

---

## 🔍 Algorithms Implemented

### 1️⃣ SIFT Algorithm
**Purpose:**  
To detect and match keypoints between two images that may have different scales, rotations, or lighting.

**Key Features:**
- Detects distinctive and scale-invariant keypoints.
- Descriptors are robust to image transformation.
- Matches keypoints between two images using descriptor similarity.

**Use Case:**  
Ideal for recognizing the same object or scene in different conditions or from different angles.

---

### 2️⃣ RANSAC for Outlier Removal
**Purpose:**  
To filter out incorrect keypoint matches (outliers) and estimate a reliable transformation (homography) between two images.

**How It Works:**
- Repeatedly selects random subsets of matches.
- Fits a transformation model (like homography).
- Chooses the best model that has the highest number of inliers.

**Use Case:**  
Crucial in tasks like panorama creation where some matches may be incorrect or noisy.

---

### 3️⃣ Harris Corner Detector
**Purpose:**  
To detect corner points in a grayscale image based on local intensity changes.

**How It Works:**
- Computes image gradients.
- Evaluates a matrix (Harris matrix) for each pixel.
- Corners are detected where there’s a large variation in all directions.

**Use Case:**  
Used in real-time tracking and motion detection due to its computational efficiency.

---

### 4️⃣ Shi-Tomasi Corner Detector
**Purpose:**  
Improves upon Harris Corner Detector by using a more stable measure of corner quality.

**Key Features:**
- Selects corners with high-quality eigenvalues.
- Returns strong and well-distributed feature points.

**Use Case:**  
Frequently used in feature tracking (e.g., Lucas-Kanade Optical Flow).

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
