# 🚗 Road Accident Risk Predictor

An end-to-end **Machine Learning** project that predicts the likelihood of road accidents based on driving conditions, driver behavior, vehicle information, and environmental factors. The project compares multiple classification algorithms and provides an interactive **Gradio** web application for real-time accident risk prediction.

---

## 📖 Project Overview

Road accidents are influenced by several factors, including weather conditions, road surface, driver experience, vehicle speed, and traffic density. This project analyzes these factors using Machine Learning to predict whether an accident is likely to occur.

The project covers the complete Machine Learning pipeline:

- Data Loading
- Exploratory Data Analysis (EDA)
- Data Cleaning & Preprocessing
- Feature Engineering
- Model Training
- Model Evaluation
- Model Comparison
- Model Deployment using Gradio

---

## ✨ Features

- 📊 Exploratory Data Analysis (EDA)
- 🧹 Data preprocessing and cleaning
- ⚙️ Feature engineering
- 🤖 Multiple Machine Learning models
- 📈 Performance comparison
- 💾 Model serialization using Pickle
- 🌐 Interactive Gradio web application
- 🎯 Real-time accident risk prediction
- 📉 Probability score for predictions
- 💡 Safety recommendations based on user inputs

---

## 📂 Dataset

The project uses a dataset containing **6,000 records** with information related to:

| Feature | Description |
|----------|-------------|
| Road Type | Highway, Urban, Rural, Residential |
| Weather | Clear, Rainy, Foggy, Snowy, Windy |
| Visibility | Visibility in kilometers |
| Road Surface | Dry, Wet, Icy, Muddy |
| Light Condition | Daylight, Dark Lit, Dark Unlit, Dusk |
| Vehicle Speed | Speed in km/h |
| Traffic Density | Low, Medium, High |
| Vehicle Type | Car, Bus, Truck, Motorcycle |
| Driver Age | Driver's age |
| Driver Experience | Driving experience in years |
| Alcohol Consumption | Yes / No |
| Seat Belt | Yes / No |
| Time of Day | Morning, Afternoon, Evening, Night |
| Day of Week | Monday–Sunday |
| Area Type | Urban / Rural |
| Road Curvature | Straight, Slight Curve, Sharp Curve |
| Junction Type | No Junction, T-Junction, Crossroad, Roundabout |
| Traffic Signal | Yes / No |
| Pedestrian Crossing | Yes / No |
| Rain | Yes / No |
| Fog | Yes / No |
| Temperature | Temperature (°C) |

**Target Variable**

- **Accident_Occurred**
  - 0 → No Accident
  - 1 → Accident

---

# 🧠 Machine Learning Models

The following supervised learning models were trained and evaluated:

## 1. XGBoost Classifier

Extreme Gradient Boosting is an ensemble learning algorithm that builds decision trees sequentially, improving performance by correcting previous errors.

### Advantages

- High prediction accuracy
- Handles non-linear relationships
- Works well on structured datasets
- Resistant to overfitting

---

## 2. Gradient Boosting Classifier

Gradient Boosting combines multiple weak decision trees into a strong predictive model.

### Advantages

- High accuracy
- Robust performance
- Handles complex datasets

---

## 3. K-Nearest Neighbors (KNN)

KNN is a distance-based algorithm that classifies a sample according to the majority class among its nearest neighbors.

### Parameters

- Number of neighbors (K) = **7**

---

# 📊 Model Evaluation

Each model was evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix
- ROC Curve
- AUC Score

---

# ⚙️ Project Workflow

```
Dataset
     │
     ▼
Data Cleaning
     │
     ▼
Exploratory Data Analysis
     │
     ▼
Feature Engineering
     │
     ▼
Encoding & Scaling
     │
     ▼
Model Training
     │
     ▼
Model Evaluation
     │
     ▼
Model Comparison
     │
     ▼
Save Best Models
     │
     ▼
Gradio Web Application
```

---

# 🔧 Feature Engineering

The following new features were created:

- Speed_Over_Limit
- Experience_Ratio
- Low_Visibility_Flag

These engineered features improve the predictive capability of the models.

---

# 🛠 Technologies Used

| Technology | Purpose |
|------------|---------|
| Python | Programming Language |
| NumPy | Numerical Computation |
| Pandas | Data Processing |
| Matplotlib | Data Visualization |
| Seaborn | Statistical Visualization |
| Scikit-learn | Machine Learning |
| XGBoost | Gradient Boosting Algorithm |
| Pickle | Model Saving |
| Joblib | Serialization |
| Gradio | Interactive Web Interface |

---

# 📁 Project Structure

```
road-accident-risk-predictor/
│
├── app.py
├── notebook.ipynb
├── requirements.txt
├── README.md
├── LICENSE
├── Road_Accident_Dataset.csv
├── scaler.pkl
├── xgb_model.pkl
├── gradient_model.pkl
├── knn_model.pkl
├── encoders.pkl
│
└── images/
    ├── banner.png
    ├── prediction.png
    └── comparison.png
```

---

# 🚀 Installation

## Clone Repository

```bash
git clone https://github.com/YourUsername/road-accident-risk-predictor.git
```

Go to project directory

```bash
cd road-accident-risk-predictor
```

Install dependencies

```bash
pip install -r requirements.txt
```

Run the application

```bash
python app.py
```

---

# 💻 Running in Google Colab

1. Open the notebook.
2. Upload the dataset.
3. Run all notebook cells.
4. Wait until Gradio generates a public link.
5. Open the generated link in your browser.

---

# 📊 Results

The notebook automatically compares all trained models.

Example metrics:

| Model | Accuracy | Precision | Recall | F1 Score |
|---------|----------|-----------|--------|----------|
| XGBoost | Best Model | - | - | - |
| Gradient Boosting | - | - | - | - |
| KNN | - | - | - | - |

*(Results depend on the training run and dataset.)*

---

# 🌐 Web Application

The Gradio interface allows users to:

- Select a Machine Learning model
- Enter road and driver information
- Predict accident risk
- View prediction probability
- Compare model performance
- Receive safety recommendations

---

# 📷 Screenshots

### Home Page

> Add a screenshot here

```
images/banner.png
```

### Prediction Interface

> Add screenshot here

```
images/prediction.png
```

### Model Comparison

> Add screenshot here

```
images/comparison.png
```

---

# 📌 Future Improvements

- Deep Learning models
- Real-world accident dataset
- Explainable AI (SHAP/LIME)
- Cloud deployment
- Mobile-friendly interface
- Real-time weather API integration
- GPS-based accident prediction

---

# ⚠ Disclaimer

This project is developed for **educational and research purposes only** using a synthetically generated dataset. The predictions should **not** be used for real-world road safety decisions.

---

# 🤝 Contributing

Contributions are welcome.

If you would like to improve this project:

1. Fork the repository.
2. Create a new branch.
3. Commit your changes.
4. Open a Pull Request.

---

# 📄 License

This project is licensed under the **MIT License**.

---

# 👨‍💻 Author

WAQAS AHMED SHAHEEN
HAIDER MAQSOOD

BS Computer Science Student

Machine Learning Enthusiast

GitHub: https://github.com/YourUsername

---

## ⭐ Support

If you found this project useful, consider giving it a **⭐ Star** on GitHub.
