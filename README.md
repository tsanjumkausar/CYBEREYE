# 🛡️ CyberEye – AI-Powered Real-Time Phishing Detection

CyberEye is a real-time AI-powered phishing detection system that leverages the **Gemma LLM** for intelligent URL classification. It automatically identifies websites as **Phishing**, **Defacement**, **Malicious**, or **Benign**, providing detailed threat reasoning and maintaining a history of all scans via a Flask + SQLite backend. A Chrome Extension adds real-time scanning for open browser tabs, reducing phishing exposure by **98%**.

---

## 🧠 Classification Categories

1. **Phishing** – Pretends to be a trusted site to steal personal data (e.g., login or banking).
2. **Defacement** – A legitimate website that has been altered or defaced by hackers.
3. **Malicious** – Delivers malware, spyware, or harmful code.
4. **Benign** – Safe, trusted website with no harmful behavior.

---

## ⚙️ How It Works

1. User visits the **React frontend** and inputs a URL.
2. The URL is sent to the **Flask backend API**.
3. The **Gemma LLM model** classifies the URL and provides reasoning.
4. The classification result and reasoning are stored in a **SQLite database**.
5. The **Chrome Extension** runs in real-time to scan browser tabs for phishing/malicious links.
6. Results are displayed to the user with full scan history.

---
---

## 🔧 Backend – Flask + SQLite

### Setup

```bash
cd backend
(Optional) Create a virtual environment:

bash
Copy
Edit
# Windows
python -m venv venv
venv\Scripts\activate

# macOS/Linux
python3 -m venv venv
source venv/bin/activate
Install dependencies:

bash
Copy
Edit
pip install -r requirements.txt
Run the Backend
bash
Copy
Edit
python app.py
Runs on: http://localhost:5000

💻 Frontend – React + Tailwind CSS
Setup
bash
Copy
Edit
cd frontend
npm install
Run the Frontend
bash
Copy
Edit
npm start
Runs on: http://localhost:3000

🧩 Chrome Extension – Real-Time Tab Scanner
How to Install
Go to chrome://extensions/

Enable Developer Mode (top right)

Click Load Unpacked

Select the extension/ folder

Extension is now active and scanning browser tabs

🛠️ Tech Stack
Layer	Technologies
Backend	Python, Flask, Flask-CORS, SQLite
Frontend	React, Axios, Tailwind CSS
Extension	HTML, JavaScript, CSS
AI Model	Gemma LLM (via Together AI / GROQ API)

📸 Screenshots (Optional)
<!-- Add if needed ![Homepage](screenshots/home.png) ![Scan Result](screenshots/result.png) -->
📜 License
This project is licensed under the MIT License.
