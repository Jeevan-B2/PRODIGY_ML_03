### Image Classification (Cats vs. Dogs) using SVM

### 📌 Objective
Implement a Support Vector Machine (SVM) to classify images of cats and dogs from the Kaggle dataset.

### 📊 Dataset
The dataset used is the Microsoft Cats vs. Dogs dataset. Because SVMs require significant memory, the model was trained on a subset of 1,000 images (500 cats, 500 dogs) to prevent runtime crashes.

### 🛠️ Tools & Technologies
*   **Python**
*   **Google Colab**
*   **OpenCV (cv2)** (Image Processing)
*   **Scikit-Learn** (Machine Learning)
*   **Matplotlib** (Data Visualization)

### 🧠 Approach
1.  **Data Preprocessing:** Images are read in grayscale and resized to 64x64 pixels to reduce computational load.
2.  **Flattening:** The 2D images are flattened into 1D arrays so they can be fed into the SVM algorithm.
3.  **Normalization:** Pixel values (0-255) were normalized to a range of 0-1 by dividing by 255.0. This significantly improves SVM performance.
4.  **Model Training:** An SVM classifier was trained using the **RBF (Radial Basis Function) kernel** to handle the complex non-linear patterns of image data.
5.  **Evaluation:** The model's predictions were evaluated against the test set using accuracy score.

### 📈 Results & Insights
*   The model achieved an accuracy of approximately **55%**.
*   **Key Learning:** SVMs are not inherently designed for image classification (Convolutional Neural Networks are the industry standard). Processing raw pixels with an SVM results in moderate accuracy. However, this task successfully demonstrates the complete image preprocessing pipeline and SVM implementation.
