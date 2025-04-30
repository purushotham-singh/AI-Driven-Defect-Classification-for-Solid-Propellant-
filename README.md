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

---
## 📝 How to Run

### ✅ Choose Google Colab (Recommended)

You can run this project entirely in your browser — no setup or installation needed!

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/yourusername/AI-Driven-Defect-Classification-for-Solid-Propellant/blob/main/notebooks/Defect_Classifier_Colab.ipynb)

> 📎 _Upload your ultrasonic data CSV (with `Time` and `Amplitude` columns) when prompted._
>
> 📌 _Run all cells from top to bottom to ensure correct feature extraction, visualization, and defect classification._

---

### 🧠 Notes
- Works best with Google Chrome or Firefox
- No Python installation required
- Supports both manual uploads and Google Drive access
