# **Mycotoxin Level Prediction Using Hyperspectral Imaging**

## **Overview**
This project processes hyperspectral imaging data of corn samples to predict mycotoxin (DON) concentration. The workflow includes data preprocessing, dimensionality reduction using PCA, training a **Random Forest Regressor**, and evaluating its performance.

## **Dataset Description**
- **Features**: Spectral reflectance values across multiple wavelength bands.
- **Target Variable**: DON concentration (continuous) for regression.
- **Rows**: Individual corn samples.


## **Installation & Setup**
1. Clone the repository:
   ```
   git clone https://github.com/aakarsh1227/ImageIo.git
   cd ImageIo
   ```
2. Install dependencies:
```sh
pip install -r requirements.txt
```
3. (Optional) Create a virtual environment:
```
python -m venv env
source env/bin/activate   # On Windows: env\Scripts\activate
```


## **Workflow**
### **1. Data Preprocessing**
- Checked and confirmed no missing values.
- Removed the **hsi_id** column as it was not relevant.
- Applied **StandardScaler** for normalization of spectral features.

### **2. Dimensionality Reduction**
- Used **Principal Component Analysis (PCA)** for dimensionality reduction.
- Retained top components explaining significant variance.
- Visualized results with a **scatter plot of the first two principal components**.

### **3. Model Training & Evaluation**
- **Model Used**: **Random Forest Regressor**
- **Hyperparameters**: Default settings with **100 trees**.
- **Performance Metrics**:
  - **Mean Absolute Error (MAE)**: Computed and reported in script.
  - **Root Mean Squared Error (RMSE)**: Computed and reported in script.
  - **R² Score**: Computed and reported in script.
- **Visualizations**:
  - Scatter plot of **actual vs. predicted DON concentration**.

### **4. Key Findings & Suggestions for Improvement**
- **Random Forest performed reasonably well**.
- Advanced models like **XGBoost or deep learning (CNN/LSTM)** could further improve accuracy.
- **Hyperparameter tuning (GridSearch or RandomSearch)** could optimize performance.
- **Exploring t-SNE** for better visualization of data clustering might provide deeper insights.

## **Results & Findings**
- **PCA results**: Explained variance captured in top components.
- **Random Forest model performance**: Regression metrics and visualization.
- **Recommendations**: Future improvements using deep learning models.

## **Future Improvements**
- Implement an **XGBoost model** to compare performance.
- Fine-tune **Random Forest hyperparameters** for better accuracy.
- Explore **t-SNE visualization** for deeper insights.
- Build an **interactive Streamlit app** for real-time predictions.

---

## **Author**
👤 **Aakarsh Mishra**  
📧 Email: [aakarshmishra1227@gmail.com](mailto:aakarshmishra1227@gmail.com)  
🔗 LinkedIn: [Aakarsh Mishra's LinkedIn](https://www.linkedin.com/in/aakarshmishra1227/)
