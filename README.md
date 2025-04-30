# AI-Driven Defect Classification for Solid Propellant

This project aims to automate the defect identification and classification process in solid propellant rocket motors using ultrasonic testing data and AI/ML algorithms. It processes time-series amplitude signals to detect and categorize defects that arise due to manufacturing, environmental, or chemical issues.

---

## 🚀 Project Objective

To develop a robust, AI-powered pipeline that analyzes ultrasonic signal data from solid propellant motors to:

- Identify the presence of defects
- Classify the type of defect (natural, climate-induced, environmental, or chemical)
- Visualize important signal features (TOF, Tp, FFT, etc.)
- Provide statistical summaries and classification confidence

---

## 🧠 Technologies Used

- **Python 3.10+**
- **NumPy**, **Pandas** – Data manipulation
- **Matplotlib**, **Seaborn**, **Plotly** – Visualization
- **SciPy** – Signal processing
- **Scikit-learn** – Machine Learning
- **TensorFlow / PyTorch** (optional) – Deep Learning Models
- **Jupyter Notebooks** – Experimentation & Visualization

---

## 📂 Dataset

- **Input Format**: CSV files with `Time` and `Amplitude` columns
- **Sampling Rate**: ∆t = 0.5 seconds
- **Data Points**: ~3000 values per test sample
- **Features Extracted**:
  - `T0`, `T1` (TOF), `Tp`, `Tr`
  - `Ap`, `Ar`
  - `FFT Frequency`, `FFT Magnitude`
  - `Signal Cycles`, `Standard Deviation`, `Mean`

---

## ⚙️ How It Works

1. **Preprocessing**: Cleans and normalizes amplitude-time data.
2. **Feature Extraction**: Calculates physical and frequency-domain features.
3. **Defect Detection**:
   - Uses a rule-based hybrid logic to initially tag data
   - Trains an ML/DL model to classify into:
     - No Defect
     - Natural Defect
     - Climate-Based Defect
     - Environmental Defect
     - Chemical Defect
4. **Visualization**: Signal curves, FFT, and time-based events.
5. **Prediction Output**: Class with confidence score.

---

## 📊 Outputs

- **Graphs**: TOF pulses, FFT spectrum, amplitude trends
- **Tables**: Extracted feature values per sample
- **Predictions**: JSON/CSV output with defect class and metrics

---## 📝 How to Run

### ✅ Use Google Colab (Recommended)

This project is designed to run seamlessly on **Google Colab**, allowing you to analyze ultrasonic defect data without any local setup.

> 🚀 Simply open the `.ipynb` notebook located in the `notebooks/` folder using **Google Colab** (Right-click → Open with → Colab).

> 📎 Upload your own CSV file containing `Time` and `Amplitude` columns when prompted.

> ✅ Run all cells in sequence to perform:
> - Signal preprocessing
> - Feature extraction (TOF, Tp, FFT, etc.)
> - Defect classification using AI/ML models
> - Visualization of results

---

### 📌 Why Colab?
- No installation or configuration needed
- Runs in the cloud, works on any device
- Ideal for experimenting with Jupyter notebooks and datasets
