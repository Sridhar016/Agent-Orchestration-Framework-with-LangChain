# 🏥 MedAgentApp — AI Medical Report Analyzer  

![Open in Streamlit](https://medagentapp-cn5gdssn2dsvp9kbdhqehz.streamlit.app/)  

---

### 🧬 Overview  
**MedAgentApp** is a modern, intelligent medical report analyzer built with **Streamlit** and **Google Gemini 2.5 Flash**.  
It’s designed for **healthcare education, research, and diagnostic assistance**, offering:  
- A clean, card-based interface  
- Real-time AI-powered analysis  
- Secure API key handling  
- Local report history tracking  

---

## 🧠 Example Use Case  

**Input:**  
Patient: Riya Sharma
Age: 28
Symptoms: Fever, cough, mild fatigue


**AI Diagnosis Output:**  
🩺 **Diagnosis Summary:**  
- Possible mild viral infection (upper respiratory)  
- Recommend rest, fluids, and paracetamol  
- If cough persists >5 days, follow up for bacterial screening  

⚠️ *Note: This output is advisory only — not a medical prescription.*

---

## ⚙️ Setup Instructions  

### 1️⃣ Clone the Repository  

git clone https://github.com/YOUR-USERNAME/MedAgentApp.git
cd MedAgentApp

2️⃣ Create and Activate a Virtual Environment

python -m venv venv
venv\Scripts\activate        # For Windows

# or
source venv/bin/activate     # For macOS/Linux

3️⃣ Install Required Packages

pip install -r requirements.txt

4️⃣ Add Your Gemini API Key Securely

Create a file named .env in the same folder as app.py and add your Gemini API key:

GOOGLE_API_KEY=your_actual_api_key_here

⚠️ Never upload your .env file to GitHub — it’s already protected in .gitignore.

5️⃣ Run the Application

streamlit run app.py

Now open your browser and visit 👉 http://localhost:8501

---

☁️ Deployment (Streamlit Cloud)

1️⃣ Push your code to GitHub

2️⃣ Go to https://share.streamlit.io

3️⃣ Connect your GitHub repo → click Deploy

4️⃣ Go to Settings → Secrets → Add New Secret

Key: GOOGLE_API_KEY
Value: your Gemini API key

✅ This keeps your key secure — it’s never visible in the public repo.

5️⃣ Click Save & Rerun — your app is now live 🌐🎉

---

🔒 Security and Privacy

✅ Your Gemini API key is stored only in .env (local) or Streamlit Secrets (cloud).

✅ User reports are stored locally (diagnosis_logs_json/) for personal access.

✅ No medical data is shared externally except for Gemini analysis calls.

---
🧰 Project Structure
```
📁 MEDICAL/
├── app.py                # 🎯 Main Streamlit web app
├── agent.py              # 🤖 Gemini AI logic & multi-agent analysis
├── .env                  # 🔑 API key (secure, ignored by Git)
├── .gitignore            # 🚫 Prevents secret uploads
├── requirements.txt      # 📦 All dependencies
├── diagnosis_logs/       # 📄 AI-generated reports (PDF)
├── diagnosis_logs_json/  # 🧠 JSON logs per user
└── vector_db/            # ⚙️ Optional embeddings / cache
```
---

🧾 Example Output

Smooth, responsive Streamlit UI

Sidebar navigation for Report & Analyze, Follow-up, and Download Report

Real-time AI agent animation (“🧠 Agent analyzing...”)

Downloadable PDF reports

Stored analysis history for personalized follow-ups

---

🚀 Future Enhancements

🧬 Integration with wearable devices (Fitbit, Apple Health)

📊 Symptom tracking dashboard

🌍 Multi-language report analysis

🧠 Offline AI diagnosis (local LLM support)

🕵️ Doctor Portal for AI-reviewed case histories

---

⚠️ Disclaimer

This tool is built for educational and research purposes only.
It is not a certified medical device or substitute for a licensed healthcare professional.
Always consult a doctor for real medical advice or treatment.

---

👩‍💻 Author

Maheswari G

---

💖 Acknowledgements

Special thanks to:

Google DeepMind — Gemini API

Streamlit Team — for the open-source platform

OpenAI & LangChain Community — for developer inspiration




