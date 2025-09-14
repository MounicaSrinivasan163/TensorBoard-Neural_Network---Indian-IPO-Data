# TensorBoard-Neural_Network---Indian-IPO-Data

Predicting the long-term gains of IPOs using machine learning and deep learning models.

---

## Project Overview

This project builds a regression model to predict **Current Gains** of IPOs based on IPO-related features such as issue size, investor subscriptions, offer price, and listing price. The goal is to help investors understand potential returns using historical IPO data.

**Key highlights:**

- Data preprocessing including scaling and handling missing values.
- Neural network regression using TensorFlow/Keras.
- Custom metrics: RMSE and R².
- TensorBoard integration for monitoring training and validation metrics.
- Chronological validation to avoid target leakage.

---

## Dataset

The dataset includes the following features:

| Column | Description |
|--------|-------------|
| Date | IPO listing date |
| IPO_Name | IPO identifier |
| Issue_Size(crores), QIB, HNI, RII, Total | Investor subscription details |
| Offer Price, List Price | Price details at IPO and listing |
| Listing Gain | Gain on listing day |
| CMP(BSE), CMP(NSE) | Current market price |
| Current Gains | **Target variable** — long-term gains |

> **Note:** Only features known before IPO are used for predictions to prevent leakage.

---

## Installation

Clone the repository and install dependencies:

- Python 3.9+
- TensorFlow 2.x
- Pandas
- Numpy
- Scikit-learn
- Matplotlib / Seaborn (optional for plotting)
- TensorBoard

---

## Usage

1. **Data Preprocessing**  
   - Handle missing values and clean the dataset.  
   - Select relevant features available before IPO to prevent target leakage.  
   - Scale features for neural network training.

2. **Training the Neural Network**  
   - Split data chronologically for training and validation.  
   - Train a neural network model to predict `Current Gains`.

3. **TensorBoard for Monitoring**  
   - TensorBoard is used to **visualize training and validation metrics** over epochs.  
   - You can track loss, RMSE, and R² in real time to monitor model performance and detect overfitting.  
   - It can be launched inside Colab or exposed via a public URL for interactive moni

