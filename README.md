# Liver Cirrhosis Outcome Prediction – Deep Neural Network

This project implements a **Deep Neural Network (DNN)** model to predict the prognosis of liver cirrhosis patients using clinical and biochemical data.  
The dataset was preprocessed to handle missing values, outliers, and categorical encoding before training the model.

---

## 📊 Data Preprocessing
- **Removed duplicates** and cleaned text data.
- **Handled missing values**:
  - Numerical columns → replaced with mean.
  - Categorical columns → replaced with mode.
- **Outlier removal** using the IQR method.
- **One-hot encoding** for categorical variables.
- **Standardization** of features using `StandardScaler`.
- Performed **80/20 train-test split** with stratification.

---

## 🧠 Model – Deep Neural Network
- Implemented using **Keras** with TensorFlow backend.
- Architecture:
  - Input layer matching number of features.
  - Multiple hidden layers with **ReLU activation**.
  - **Dropout** layers for regularization.
  - Output layer with **softmax activation** for multi-class classification.
- Optimized with **Adam** optimizer.
- Used **categorical crossentropy** as the loss function.
- **Early Stopping** to prevent overfitting.

---

## 📈 Model Performance
- **Accuracy:** ~92%
- **Weighted F1-score:** ~0.92
- Model showed balanced performance across all classes despite class imbalance.

---

## 📂 Repository Structure
-├── liver_cirrhosis_dnn.ipynb # Jupyter Notebook with full implementation
-├── README.md # Project documentation
-└── data/ # Dataset (if included)
