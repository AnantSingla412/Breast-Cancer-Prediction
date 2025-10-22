🧠 AI Web Application — Local & AWS Deployment Guide
📂 Project Overview

This project consists of a Flask-based web application for AI model deployment and testing.
It includes two main environments:

Local Development → Using app.py and the templates/ folder

Cloud Deployment → Using testai folder (a slightly modified version) hosted on an AWS EC2 instance

⚙️ Local Setup
1. Folder Structure
Breast-Cancer-Prediction/
│
├── app.py
├── templates/
│   ├── home.html
└── requirements.txt

2. How to Run Locally

Clone or download the project folder.

Navigate to the project directory:

cd Breast-Cancer-Prediction


Install required libraries:

pip install -r requirements.txt


Run the Flask app:

python app.py


Open your browser and go to:

http://127.0.0.1:5000

☁️ AWS Deployment

1. Folder Structure
Breast-Cancer-Prediction/
testai/
│
├── app.py
├── templates/
│   ├── home.html
└── requirements.txt

1. Files Used

Modified version of app.py for AWS hosting

Deployment Notes → Contained in the provided PDF file

2. Tools Used

AWS EC2 Instance

PuTTY → For SSH access and running commands on the instance

WinSCP → For transferring project files between local system and EC2 instance

3. Deployment Steps (as per PDF notes)

Connect to your EC2 instance using PuTTY.

Transfer files (app.py, templates/, and dependencies) or testai folder to the server using WinSCP.

Install Python dependencies on the instance.

Run the Flask application on a public IP/port.

Access the deployed app through your EC2 Public IPv4 DNS or Elastic IP.

📝 Notes

The templates/ folder and app.py work seamlessly in the local environment.

The testai  version is optimized for AWS deployment with minor adjustments for server compatibility.

Refer to the attached deployment PDF for complete step-by-step details.

🧩 Tech Stack

Backend: Flask (Python)

Hosting: AWS EC2

Tools: PuTTY, WinSCP
