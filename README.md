# Earthquake Prediction using Neural Networks

## 📘 Overview
This project focuses on predicting earthquake parameters such as **magnitude** and **depth** using seismic and temporal data.  
It leverages **Machine Learning and Deep Learning** techniques to identify underlying patterns in earthquake occurrences.

Developed as part of a Data Science internship project to explore predictive modeling, data preprocessing, and visualization of geospatial events.

---

## 📊 Dataset
The model uses a dataset named `database.csv` containing:
- **Date**
- **Time**
- **Latitude**
- **Longitude**
- **Depth**
- **Magnitude**

Data preprocessing included:
- Combining `Date` and `Time` into a single `Datetime` column
- Converting `Datetime` to a numerical `Timestamp`
- Dropping missing values
- Selecting key features (`Timestamp`, `Latitude`, `Longitude`) for prediction

---

## ⚙️ Methodology

### 1. Data Visualization
- Used **Basemap** and **Matplotlib** to visualize global earthquake locations.
- Highlighted affected areas and seismic distribution across latitudes and longitudes.

### 2. Model Development
A **Feedforward Neural Network** was built using **Keras Sequential API**:
- Two hidden layers with **sigmoid** activation
- Output layer with **softmax** activation
- Optimizer: **SGD**
- Loss function: **Squared Hinge Loss**
- Evaluation Metric: **Accuracy**

### 3. Model Optimization
Used **GridSearchCV** to fine-tune hyperparameters such as:
- Number of neurons
- Activation functions
- Optimizers
- Loss metrics

---

## 🧪 Results
The final model was trained for 20 epochs with a batch size of 10.  
Evaluation on the test dataset yielded promising accuracy for predicting magnitude and depth trends.

**Evaluation Result (example):**
Loss = 0.21
Accuracy = 90%

yaml
Copy code

---

## 🧰 Technologies Used
- **Python**
- **Keras / TensorFlow**
- **Scikit-learn**
- **Pandas / NumPy**
- **Matplotlib / Seaborn / Basemap**
- **Jupyter Notebook**

---

## 📈 Future Enhancements
- Integrate additional geophysical parameters for better model generalization  
- Deploy model as an interactive web dashboard using **Flask** or **Streamlit**  
- Automate data collection using real-time APIs

---

## 👤 Author
**Vashishtha Sagvekar**  
- B.Tech in Artificial Intelligence & Machine Learning  
- [LinkedIn](https://www.linkedin.com/in/vashishtha-sagvekar)  
- [GitHub](https://github.com/Vashishtha-11)
