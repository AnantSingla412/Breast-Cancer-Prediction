
# 🧠 AI Web Application — Local & AWS Deployment Guide

---

## 📂 Project Overview

This project consists of a **Flask-based web application** for AI model deployment and testing.
It includes two main environments:

* 🧪 **Local Development** → Using `app.py` and the `templates/` folder
* ☁️ **Cloud Deployment** → Using the `testai` folder (a slightly modified version) hosted on an **AWS EC2 instance**

---

## ⚙️ Local Setup

### **1. Folder Structure**

```
Breast-Cancer-Prediction/
│
├── app.py
├── templates/
│   ├── home.html
└── requirements.txt
```

---

### **2. How to Run Locally**

1. **Clone or download** the project folder.
2. **Navigate** to the project directory:

   ```bash
   cd Breast-Cancer-Prediction
   ```
3. **Install required libraries:**

   ```bash
   pip install -r requirements.txt
   ```
4. **Run the Flask app:**

   ```bash
   python app.py
   ```
5. **Open your browser** and go to:

   ```
   http://localhost:5000
   ```

---

## ☁️ AWS Deployment

### **1. Folder Structure**

```
Breast-Cancer-Prediction/
│
└── testai/
    ├── app.py
    ├── templates/
    │   ├── home.html
    └── requirements.txt
```

---

### **2. Files Used**

* **Modified version of `app.py`** for AWS hosting
* **Deployment Notes** → Contained in the provided **PDF file**

---

### **3. Tools Used**

| Tool                 | Purpose                                             |
| -------------------- | --------------------------------------------------- |
| **AWS EC2 Instance** | Cloud hosting platform                              |
| **PuTTY**            | SSH access and command execution                    |
| **WinSCP**           | File transfer between local system and EC2 instance |

---

### **4. Deployment Steps (as per PDF notes)**

1. Connect to your **EC2 instance** using **PuTTY**.
2. Transfer files (`app.py`, `templates/`, and dependencies) or the **`testai`** folder to the server using **WinSCP**.
3. Install Python dependencies on the EC2 instance.
4. Run the Flask application on a public IP/port.
5. Access the deployed app through your **EC2 Public IPv4 DNS** or **Elastic IP**.

---

## 📝 Notes

* The **`templates/`** folder and **`app.py`** work seamlessly in the **local environment**.
* The **`testai`** version is optimized for **AWS deployment** with minor adjustments for server compatibility.
* Refer to the attached **deployment PDF** for complete step-by-step setup details.

---

## 🧩 Tech Stack

| Component   | Technology     |
| ----------- | -------------- |
| **Backend** | Flask (Python) |
| **Hosting** | AWS EC2        |
| **Tools**   | PuTTY, WinSCP  |


