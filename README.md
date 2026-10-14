# 🔐 Session Hijacking Detection System (Capstone Project)

# 📌 Project Overview
The **Session Hijacking Detection System** is a web-based security tool designed to analyze a website’s **session management**, **security headers**, and other vulnerabilities. It uses machine learning to classify websites as **Secure**, **Insecure**, or **Highly Insecure**.

### Core Workflow:
1. Information gathering (headers, cookies, metadata)  
2. Detection of vulnerabilities  
3. Identification of potential attack vectors  
4. Creation of a custom dataset using real scans (e.g. UOS, Thal University)  
5. Training of multiple ML models  
6. Comparison of manual vs. model-based results  
7. Real-time URL scanning with detailed security reports  


## 🚀 Features
- **Information Gathering:** Retrieve metadata, cookies, and headers of the website  
- **Vulnerability Detection:** Check for weak session tokens, missing headers, etc.  
- **Attack Vector Identification:** List possible types of session hijacking attempts  
- **Dataset Creation:** Build dataset from real-world website scans

  
- **ML Models Used:**  
  - Random Forest Classifier  
  - Decision Tree Classifier  
  - **XGBoost** (best performing)
    
- **Performance Comparison:** Validate predictions by contrasting with manual results  
- **Live Security Scan:** Enter any URL and immediately get a detailed security analysis  

## 🛠️ Tech Stack
- **Frontend:** HTML, CSS, JavaScript  
- **Backend:** Python (Flask)  
- **Machine Learning:** Random Forest, Decision Tree, XGBoost  
- **Dependencies:**
  - scikit-learn
  - xgboost
  - pandas
  - numpy
  - joblib
  - tldextract
  - requests

## 📂 Project Flow
1. Gather site data (headers, cookies, metadata)  
2. Detect session hijacking–related vulnerabilities  
3. Identify attack routes  
4. Build dataset from UOS, Thal, and other sites  
5. Train ML models and select the best (XGBoost)  
6. Compare model predictions with manual tests  
7. Deploy as Flask web app for real-time scanning  


## 📊 Dataset Details
- **Source:** Self-created via real website scans  
- **Features:** ~34 features including headers, cookie flags, SSL info  
- **Target:** `Security_Class` (Secure, Insecure, Highly Insecure)  
- **Preprocessing Steps:** Missing value handling, encoding, scaling, and SMOTE-based balancing  


## 🧠 Model Performance

| Model                      | Accuracy  | Performance Notes              |
|----------------------------|-----------|---------------------------------|
| Random Forest Classifier   | Good      | Reliable, but not the best      |
| Decision Tree Classifier   | Moderate  | Simple but less accurate        |
| **XGBoost Classifier**    | ⭐ Best   | Highest accuracy observed       |


# ⚙️ Installation & Run Instructions

# Clone the repository
git clone https://github.com/HadiaWaheed/capstoneProject.git

# Navigate into the project folder
cd capstoneProject

# Install dependencies
pip install -r requirements.txt

# Run the Flask app
python app.py




---

## 📸 Project Screenshots

This section showcases the screenshots of the Session Hijacking Detection System, including secure and insecure website analysis, security checks, and model comparisons.

### 1. Secure Website Detection
![Secure Website](Documentation%20of%20FYP/images/secure.png)

### 2. Secure Google Analysis
![Secure Google](Documentation%20of%20FYP/images/secure%20google.png)

### 3. Secure URL Analysis
![Secure URL](Documentation%20of%20FYP/images/secure%20url.png)

### 4. Insecure Website Detection
![Insecure Website](Documentation%20of%20FYP/images/insecure.png)

### 5. Highly Insecure URL Detection
![Highly Insecure URL](Documentation%20of%20FYP/images/high%20insecure%20url.png)

### 6. CMIT Insecure Analysis
![CMIT Insecure](Documentation%20of%20FYP/images/CMIT%20insecure.png)

### 7. CMIT Security Check
![CMIT Check](Documentation%20of%20FYP/images/CMIT%20check.png)

### 8. Model Comparison
![Model Comparison](Documentation%20of%20FYP/images/Comparison.png)

### 9. Additional Model Comparison
![Another Comparison](Documentation%20of%20FYP/images/Another%20comparision.png)

### 10. Application Screenshot
![Application Screenshot](Documentation%20of%20FYP/images/14.10.2026_13.20.15_REC.png)

