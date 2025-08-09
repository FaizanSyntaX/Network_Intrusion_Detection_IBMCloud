# 🚀 Network Intrusion Detection System (NIDS) using IBM AutoAI

## 📌 Project Overview
This project is part of my **IBM SkillsBuild Internship** and focuses on building a **Network Intrusion Detection System (NIDS)** using **IBM Watson AutoAI** on **IBM Cloud Lite**.

The system:
- Analyzes network traffic data
- Detects multiple types of cyber-attacks:
  - DoS (Denial of Service)
  - Probe
  - R2L (Remote-to-Local)
  - U2R (User-to-Root)
- Differentiates between normal and malicious activity
- Provides **real-time predictions** via an API

---

## 📂 Dataset Details
- **Name:** Intrusion Detection Dataset (KDD/NSL-KDD format)
- **File:** `Train_data.csv` (Training) & `Test_data.csv` (Testing)
- **Records:** ~125,973 entries
- **Features:** 41 attributes (network connection details)
- **Target Variable:** `class` (Normal, DoS, Probe, R2L, U2R)

---

## 🛠 Tools, Libraries, and Services Used

### 1. **IBM Cloud Services**
- IBM Cloud Lite Account
- IBM Watson Studio
- IBM Watson Machine Learning (WML)
- IBM Cloud Object Storage
- IBM AutoAI
- Watson ML Runtime Environment

### 2. **Programming Language**
- Python 3.x

### 3. **Python Libraries** (for optional local testing)
- `pandas` – CSV dataset handling
- `scikit-learn` – Additional evaluation
- `requests` – For API interaction (optional)
- `json` – For handling JSON data (optional)

### 4. **External Tools**
- Google Chrome – For IBM Cloud access
- Visual Studio Code – For Python scripting
- Git & GitHub – For version control

---

## 🖥 System Requirements

**Hardware:**
- CPU: Intel Core i5 or higher
- RAM: 8 GB minimum
- Storage: 2 GB free space
- Internet: Stable broadband connection

**Software:**
- IBM Cloud account (Lite plan)
- Modern web browser (Google Chrome recommended)
- Python 3.x installed locally (optional)

---

## 📜 Project Workflow

1. **Upload Dataset**
   - Upload `Train_data.csv` to IBM Cloud Object Storage via Watson Studio project assets.

2. **Create AutoAI Experiment**
   - Select dataset from project
   - Set target column: `class`
   - Problem type: Classification

3. **Run Experiment**
   - AutoAI handles:
     - Data preprocessing
     - Feature engineering
     - Model selection
     - Hyperparameter tuning

4. **Select Best Model**
   - Based on highest F1-score & accuracy
   - Example: Random Forest Classifier

5. **Save & Deploy**
   - Save the model to project assets
   - Create an **Online Deployment** in Watson Machine Learning

---

## 📊 Model Performance
- **Best Model:** XGB Classifier (AutoAI Pipeline-15)
- **Accuracy:** 99.8%
- **F1-score:** 0.998
- **Precision:** 0.996
- **Recall:** 0.999

---

## 📷 Screenshots

<img width="1920" height="1080" alt="Screenshot (178)" src="https://github.com/user-attachments/assets/6edb56b0-ab36-4ad4-9ea7-4c5402a8ee62" />
<img width="1920" height="1080" alt="Screenshot (152)" src="https://github.com/user-attachments/assets/fea8b152-1d24-48b5-bf77-0eb4c2e75370" />
1. Dataset uploaded in Watson Studio  
<br>
<img width="1920" height="1080" alt="Screenshot (110)" src="https://github.com/user-attachments/assets/b6f0fd05-8a40-481e-9624-3cc1fa89a89e" />
2. AutoAI experiment creation screen  
<br>
<img width="1920" height="1080" alt="Screenshot (165)" src="https://github.com/user-attachments/assets/2e31b72b-df27-4675-a9f9-86d88f78e9f5" />
<img width="1867" height="512" alt="Screenshot (172)" src="https://github.com/user-attachments/assets/0b607785-c760-472b-8391-d5c7c9b784bd" />
<img width="1862" height="357" alt="Screenshot (173)" src="https://github.com/user-attachments/assets/4c777940-8c86-4bf6-823d-11b04abea8d8" />
<img width="1867" height="361" alt="Screenshot (174)" src="https://github.com/user-attachments/assets/5639017b-3d3e-49bf-b443-aac7fbcb0225" />
<img width="1865" height="355" alt="Screenshot (175)" src="https://github.com/user-attachments/assets/11418453-2a2c-4e69-94ea-20154e228adf" />

3. AutoAI Progress map & Pipeline leaderboard  
<br>





<img width="627" height="621" alt="image" src="https://github.com/user-attachments/assets/ce9a818f-cfdf-47f0-bd7d-7f8089e1ed8b" />
<img width="1278" height="576" alt="Screenshot (180)" src="https://github.com/user-attachments/assets/fa070817-2e99-45a1-b51c-b47dd2cf032f" />
4. Best pipeline evaluation (confusion matrix, ROC curve)  
<br>
<img width="1920" height="1080" alt="Screenshot (192)" src="https://github.com/user-attachments/assets/ca0f3c7b-c836-4d07-89f9-ba8047b2bf78" />
7. Model saved in assets  
<br>
<img width="1920" height="1080" alt="Screenshot (184)" src="https://github.com/user-attachments/assets/c244d80b-10c4-4563-a82d-09486dce04fa" />
<img width="1920" height="1080" alt="Screenshot (185)" src="https://github.com/user-attachments/assets/24f7c3e3-ff38-4bdf-b565-594233b0fd94" />
8. Deployment creation screen  
<br>
<img width="1920" height="1080" alt="Screenshot (187)" src="https://github.com/user-attachments/assets/f30f8ec1-2dbc-4364-9b39-476568fe970e" />
9. Scoring URL & API key 
<br>
<img width="1920" height="1080" alt="Screenshot (189)" src="https://github.com/user-attachments/assets/ca834062-d04d-4ff2-a30a-2b55f00f9d90" />
10. Testing

---

## 📌 Future Enhancements
- Integrate **real-time streaming** for continuous monitoring
- Use **deep learning models** for rare attack types
- Apply **class balancing** techniques to improve minority class detection

---

## 📄 License
This project is part of the **IBM SkillsBuild Internship** and is for educational purposes only.
