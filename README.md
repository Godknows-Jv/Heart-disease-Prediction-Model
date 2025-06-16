# JVCardioAI – Heart Disease Prediction Model

**JVCardioAI** is a machine learning-based heart disease prediction model trained on clinical data from the UCI Machine Learning Repository. The model evaluates a patient's risk of heart disease using various classification algorithms and standard preprocessing techniques.

## 🩺 Dataset

The dataset used for training comes from the [UCI Heart Disease Dataset](https://archive.ics.uci.edu/ml/datasets/Heart+Disease), specifically the Cleveland subset. It includes 14 clinical features such as age, sex, chest pain type, resting blood pressure, cholesterol, fasting blood sugar, and more.

The target variable indicates the presence (1) or absence (0) of heart disease.

## 🧠 Machine Learning Algorithms

Four supervised classification algorithms were trained and compared using **scikit-learn (sklearn)**:

### 1. **Logistic Regression**
- Interpretable and commonly used for binary classification problems.
- Performed moderately well but showed limitations on complex decision boundaries.

### 2. **Random Forest**
- An ensemble method based on decision trees.
- Provided improved accuracy and reduced overfitting compared to logistic regression.

### 3. **Support Vector Machine (SVM)**
- Effective in high-dimensional spaces.
- Applied with different kernel options; gave solid performance on scaled data.

### 4. **K-Nearest Neighbors (KNN)**
- Non-parametric and instance-based learner.
- Delivered the **highest accuracy of 85%**, making it the best-performing model in this project.

## ⚙️ Preprocessing

- **StandardScaler** was used to normalize the dataset before training to improve model performance.
- **Pandas & NumPy** were used for data handling and cleaning.
- **Pillow** was used for handling image-related tasks in future extensions of the project.


## 🚀 Model Deployment

The trained model is serialized using `joblib`, making it easy to load and integrate into a web, desktop, or mobile application. Here's an example code snippet to load the model:

```python
import joblib
model = joblib.load("model_knn.joblib")

# Example prediction
input_data = [29.0,2.0,130.0,204.0,202.0,0.0,0.0,1.0,0.0,3.0,0]

#Convert to numpy array and reshape for prediction
arr = np.array(input_data).reshape(1, -1)

#Scale input data using the same scaler used during training
arr_scaled = scaler.transform(arr)
arr_scaled

#Making predication
prediction = neigh.predict(arr_scaled)

#Predication Result
if prediction == 0:
    print('You are Healthy No CardioRisk.')
else:
    print('Consult your Doctor.')
print(prediction)

#output
You are Healthy No CardioRisk.
[1]







