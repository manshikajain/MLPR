# MLPR
# Face Detection and Clustering using K-Means

## Aim

The aim of this project is to detect faces from an image using Haar Cascade Classifier, classify the detected faces into clusters using K-Means clustering based on HSV color features and predict for a new face based on them.

---

## Methodology

### 1️ Face Detection
- Converted the input image to grayscale.
- Used OpenCV Haar Cascade classifier to detect faces.
- Extracted face regions from the image.

### 2️ Feature Extraction
- Converted detected face images to HSV color space.
- Extracted Hue and Saturation features.
- Created a feature matrix using these values.

### 3️ Clustering
- Applied K-Means clustering (k = 2).
- Grouped faces into two clusters based on color similarity.
- Computed cluster centroids.

### 4️ Template Classification
- Converted template image to HSV.
- Extracted hue and saturation.
- Predicted cluster using trained KMeans model.

---

## Results & Visualisation

### Cluster Scatter Plot

![Cluster Plot](images/template_output.png)

- Green points represent Cluster 0.
- Blue points represent Cluster 1.
- X markers represent centroids.
- Violet marker represents the template image.

---

### Face Detection Output

![Detected Faces](images/faces_detected.png)

---

## Key Findings

- Hue and Saturation values are effective for grouping faces based on color similarity.
- K-Means successfully separated faces into distinct clusters.
- The template image was correctly classified into its respective cluster.
- Proper feature scaling improves clustering performance.
- However, Since K means provides random initial means, everytime there would be a slight difference in clustering but the positioning of template image was altogether.

---

## Conclusion
This experiment demonstrates that unsupervised learning techniques like K-Means can effectively cluster images based on extracted features. HSV color space provides meaningful features for grouping visually similar faces.
The model successfully:
- Detected faces 
- Extracted meaningful features
- Clustered data correctly
- Predicted template class  

---

## Technologies Used

- Python
- OpenCV
- NumPy
- Matplotlib
- Scikit-learn

---

## 📁 Project Structure

