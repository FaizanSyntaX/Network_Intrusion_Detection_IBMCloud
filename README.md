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
- **Best Model:** Random Forest Classifier (AutoAI Pipeline-3)
- **Accuracy:** 98.7%
- **F1-score:** 0.986
- **Precision:** 0.987
- **Recall:** 0.986

---

## 📷 Screenshots

<img width="1920" height="1080" alt="Screenshot (152)" src="https://github.com/user-attachments/assets/fea8b152-1d24-48b5-bf77-0eb4c2e75370" />
1. Dataset uploaded in Watson Studio  

<img width="1920" height="1080" alt="Screenshot (110)" src="https://github.com/user-attachments/assets/b6f0fd05-8a40-481e-9624-3cc1fa89a89e" />
2. AutoAI experiment creation screen  

<img width="1920" height="1080" alt="Screenshot (117)" src="https://github.com/user-attachments/assets/ffcd7903-5b60-4e64-8b3d-5e6a298c2e81" />
<img width="1920" height="1080" alt="Screenshot (118)" src="https://github.com/user-attachments/assets/77520c16-526a-4c1d-bc4e-4bfa0708145d" />
3. AutoAI pipeline leaderboard  

<img width="1920" height="1080" alt="Screenshot (122)" src="https://github.com/user-attachments/assets/3c3e8ff3-e64e-4720-82f0-964533b78c74" />
<img width="1920" height="1080" alt="Screenshot (124)" src="https://github.com/user-attachments/assets/cb4b5bee-50f4-495a-bd8f-4f8b0ab779fe" />
4. Best pipeline evaluation (confusion matrix, ROC curve)  

<img width="1920" height="1080" alt="Screenshot (130)" src="https://github.com/user-attachments/assets/bd85a1de-37b3-4626-9c38-cde9ccf8c0b1" />
7. Model saved in assets  

<img width="1920" height="1080" alt="Screenshot (135)" src="https://github.com/user-attachments/assets/71f78480-bdd6-44dc-86e9-5a1e8c2664fb" />
<img width="1920" height="1080" alt="Screenshot (136)" src="https://github.com/user-attachments/assets/500fb140-547f-401a-92f9-6de8980a888f" />
8. Deployment creation screen  

<img width="1920" height="1080" alt="Screenshot (137)" src="https://github.com/user-attachments/assets/b783b1aa-c0ef-492f-842e-9811280917e1" />
9. Scoring URL & API key 

<img width="1920" height="1080" alt="Screenshot (151)" src="https://github.com/user-attachments/assets/d80680f2-14ca-40f6-810e-ab3b304f2989" />

---

## 📌 Future Enhancements
- Integrate **real-time streaming** for continuous monitoring
- Use **deep learning models** for rare attack types
- Apply **class balancing** techniques to improve minority class detection

---

## 📄 License
This project is part of the **IBM SkillsBuild Internship** and is for educational purposes only.
