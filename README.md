# Hand Gesture Classification Using MediaPipe Landmarks from the HaGRID Dataset

## Overview
This project focuses on classifying hand gestures using landmark data extracted from the **HaGRID (Hand Gesture Recognition Image Dataset)** using **MediaPipe**.

The input is a CSV file containing **x, y, and z coordinates** of hand keypoints extracted using MediaPipe. The output is a trained machine learning model that classifies gestures into predefined classes.

Through this project, we explore **data preprocessing, visualization, model training, and performance evaluation**, along with proper documentation and reproducible results.

---
## Dataset Details
The **HaGRID dataset** consists of **18 classes** of hand gestures. Each gesture is represented by **21 hand landmarks per hand** extracted using **MediaPipe**.

The CSV file contains:
- **x, y, z coordinates** for each of the 21 hand landmarks.
- **Gesture labels** corresponding to each set of landmarks.

---
## Project Deliverables
### 1. Google Colab Notebook
A well-documented **Google Colab notebook** will be uploaded to **GitHub**. The notebook includes:
- **Data Loading**: Reading the CSV file containing hand landmarks and labels.
- **Data Visualization**: Plotting keypoints for a few samples.
- **Data Preprocessing**:
  - Cleaning and normalizing data.
  - Handling missing values.
  - Splitting data into training and testing sets.
- **Model Training**:
  - Implementing at least **three** machine learning models (e.g., **Random Forest, SVM**).
  - Comparing their performance on gesture classification.
- **Evaluation**:
  - Reporting **accuracy, precision, recall, and F1-score** for each model.
- **Conclusion**:
  - Summarizing results and selecting the best-performing model.

### 2. Output Video
- A short **video demonstration** of the trained model.
- MediaPipe is used to extract hand landmarks from each frame.
- The video is uploaded to **Google Drive** with a publicly accessible link.

---
## Evaluation Criteria
1. **Code Quality**: Clean, well-documented, and reproducible.
2. **Model Performance**: Accuracy and robustness of trained models.
3. **Visualization**: Clarity and effectiveness of data and results visualization.

---
## Important Notes
- **Re-centering Hand Landmarks**:
  - Normalize **(x, y)** coordinates by making the **wrist point the origin**.
  - Divide all landmarks by the **mid-finger tip position** to ensure consistency in scale across images.
  - **z-coordinates** are pre-processed and do not need additional changes.
- **Output Stabilization**:
  - The model's output can be stabilized by taking the **mode of the predictions over a window of frames**.
- **Sharing GitHub and Video**:
  - Ensure both **GitHub repository** and **Google Drive video** links are **public** and accessible.

---
## Installation & Usage
### Requirements
Install the necessary dependencies:
```bash
pip install numpy pandas scikit-learn matplotlib mediapipe
```

### Running the Notebook
1. Open the **Google Colab Notebook**.
2. Upload the dataset CSV file.
3. Run all cells to train and evaluate the model.
4. Use the trained model to classify gestures in real-time.

---
## Author
🚀 **Developed by [_Rowaina_]**

Good luck! 🎯
