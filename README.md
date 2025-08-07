
# 🎭 KNN Face Match Classifier

This project is a hands-on implementation of the K-Nearest Neighbors (KNN) algorithm applied to face recognition. It allows users to upload an image of themselves and identifies the most visually similar actor from a dataset of 50 celebrity images using KNN-based classification.

## 📌 Project Overview

### 🔍 Objective
To classify a user-uploaded face image and find the most visually similar actor/actress in the dataset using 1-Nearest, 3-Nearest, and 5-Nearest Neighbors.

### 📷 Dataset
- **Images**: 50 colored face images (32x32 pixels) across 10 different actors (5 images per actor)
- **Format**: Each image flattened into a row of 3072 values (1024 per RGB channel)

### 🛠 Key Features
- Upload your face image and get real-time resemblance predictions
- Resize and reshape images to match dataset dimensions
- Calculate Euclidean distance between your image and all dataset images
- Visualize matched results for k=1, k=3, and k=5
- Implements majority voting scheme for multi-k matching

## 📁 File Structure

```
KNN-Face-Match-Classifier/
├── data/
│   ├── data.mat                  # Provided dataset of 50 colored images (32x32x3)
│   └── user_image.jpg            # Your own image used for matching
│
├── notebook/
│   └── KNN.ipynb                 # Main Jupyter notebook for face matching using KNN
│
├── docs/
│   └── KNN_Assignment.pdf        # Assignment instructions and background theory
│
├── outputs/
│   ├── matched_1nn.png           # Image with closest match using 1NN
│   ├── matched_3nn.png           # 3NN result (optional)
│   └── matched_5nn.png           # 5NN result (optional)
│
├── README.md                     # Project overview, usage, and documentation
├── requirements.txt              # List of Python packages used
└── .gitignore                    # Optional: Ignore runtime files (e.g., checkpoints)
```

## 🚀 How to Use

1. **Upload Files**
   - `KNN.ipynb`, `data.mat`, and your face image to your Google Drive.

2. **Run Notebook**
   - Open `KNN.ipynb` in **Google Colab**.

3. **Process Your Image**
   - Read, resize (to 32x32x3), and reshape your uploaded image.
   - Normalize the format to match dataset samples.

4. **Prediction**
   - Run 1NN to see the closest face match
   - Run 3NN and 5NN to see majority-voted predictions

## 🧪 Technologies Used
- Python (Jupyter Notebook)
- NumPy & SciPy
- OpenCV (`cv2`)
- Matplotlib (for visualization)
- Google Colab (execution platform)

## 📊 Core Concepts
- Euclidean Distance for similarity
- k-NN Classification
- Image preprocessing & reshaping
- Majority Voting

## 🧠 Learning Outcomes
- Understanding practical implementation of KNN
- Hands-on experience with facial recognition datasets
- Applying image processing and data visualization techniques
