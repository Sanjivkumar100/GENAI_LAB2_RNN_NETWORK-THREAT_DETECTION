# GENAI_LAB2_RNN_NETWORK-THREAT_DETECTION

# Network Intrusion Detection System Using LSTM Deep Learning Model

A deep learning-based **Network Intrusion Detection System (NIDS)** developed using a **Long Short-Term Memory (LSTM)** model to detect malicious network traffic and classify cyber attacks using the **NSL-KDD dataset**. 

---

## 📌 Project Overview

With the rapid growth of internet technologies, cyber attacks such as **Denial of Service (DoS)**, **Probe**, and **Remote to Local (R2L)** attacks have become major threats to network security. Traditional signature-based intrusion detection systems are unable to detect unknown or evolving attacks effectively.

This project proposes an intelligent **LSTM-based Intrusion Detection System** capable of learning patterns from network traffic data and accurately classifying malicious activities. 

---

## 🎯 Objectives

* Develop an efficient **Network Intrusion Detection System (NIDS)** using LSTM.
* Analyze and preprocess the **NSL-KDD dataset**.
* Detect and classify network traffic into:

  * Normal Traffic
  * DoS Attacks
  * Probe Attacks
  * R2L Attacks
* Improve intrusion detection accuracy using deep learning techniques.
* Evaluate model performance using:

  * Accuracy
  * Precision
  * Recall
  * F1-Score 

---

## 🛠️ Technologies Used

* Python
* TensorFlow / Keras
* NumPy
* Pandas
* Scikit-learn
* Matplotlib
* Seaborn
* Deep Learning (LSTM)

---

## 📂 Dataset

The project uses the **NSL-KDD Dataset**, an improved version of the KDD Cup 1999 dataset widely used for intrusion detection research. The dataset contains network traffic records with both normal and malicious behaviors. 

### Dataset Features

* 41 original network traffic features
* Categorical and numerical attributes
* Multiple attack categories

### Attack Classes

* Normal
* DoS
* Probe
* R2L 

---

## ⚙️ Data Preprocessing

The following preprocessing techniques are applied before training the model:

* Handling missing values
* One-Hot Encoding
* Label Encoding
* Feature Scaling using `StandardScaler`
* Reshaping data for LSTM input format

Input shape used:

```python
(samples, time_steps, features)
```

Approximate shape:

```python
(samples, 1, 122)
```



---

## 🧠 Model Architecture

The intrusion detection model is built using an **LSTM Deep Learning Architecture**.

### Architecture Flow

1. Input Layer
2. LSTM Layer (64 Units)
3. Dropout Layer
4. Dense Layer
5. Softmax Output Layer

The LSTM model helps capture sequential patterns and temporal relationships in network traffic data. 

---

## 🚀 Training Process

* Dataset split into training and testing sets (80:20 ratio)
* Optimizer: **Adam**
* Loss Function: **Sparse Categorical Crossentropy**
* Early Stopping used to prevent overfitting
* Multiple epochs used for model training 

---

## 📊 Evaluation Metrics

The model performance is evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix

These metrics help measure the effectiveness of the proposed intrusion detection system in identifying malicious network traffic. 

---

## 🏗️ System Architecture

The system follows the below workflow:

```text
NSL-KDD Dataset
       ↓
Data Preprocessing
       ↓
Feature Encoding & Scaling
       ↓
LSTM Deep Learning Model
       ↓
Attack Classification
       ↓
Prediction Output
```

The architecture diagram in the report illustrates the complete intrusion detection pipeline from data preprocessing to attack classification. 

---

## 📌 Applications

* Enterprise Network Security
* Real-Time Threat Detection
* Cloud Security Monitoring
* Cybersecurity Research
* Intrusion Monitoring Systems 

---

## ⚠️ Limitations

* Uses NSL-KDD dataset which may not fully represent modern network traffic
* Limited attack categories
* Requires high computational resources for real-time deployment
* Offline training environment 

---

## 🔮 Future Enhancements

* Use modern datasets such as **CICIDS2017**
* Implement real-time intrusion detection
* Explore Transformer-based models
* Improve computational efficiency
* Integrate with live network monitoring systems 

---

## 📈 Conclusion

This project demonstrates the effectiveness of **LSTM-based deep learning models** for detecting cyber attacks in network traffic. The proposed system improves intrusion detection accuracy and provides a strong foundation for intelligent cybersecurity solutions capable of identifying malicious activities in modern computer networks. 


