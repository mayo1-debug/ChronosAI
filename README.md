# ChronosAI
Chronos AI is a natural language scheduling assistant using OpenAI, LangChain, and Google Calendar. It turns user prompts into conflict-free events with optional fallback planning and buffer logic.



# 📄 README.md for Chronos AI

# ⏳ Chronos AI – Autonomous Scheduling Agent

Chronos AI is a natural language-powered scheduling assistant built with **OpenAI**

**LangChain**, and the **Google Calendar API**. It transforms user prompts like  
`"Schedule 3 coding sessions and 2 workouts next week"`  
into structured, conflict-free calendar events — with optional fallback times and buffer logic.

---

## 🔧 Features

- 🧠 **Natural Language Input** — Just type what you want to schedule.
- 📆 **Conflict Detection** — Automatically checks your Google Calendar for overlaps.
- 🔁 **Fallback Planning** — Suggests alternative time slots for busy days.
- ⏱️ **Buffer Management** — Adds buffer blocks between sessions.
- 💬 **Interactive Agent Flow** — Requests confirmation before final scheduling.

---

## 🚀 Quickstart

1. **Clone the repository**  
   ```bash
  git clone https://github.com/yourusername/chronos-ai.git

2.	Open Chronos_AI.ipynb in Google Colab
Make sure to upload:
	•	Your credentials.json (OAuth2 credentials from Google Cloud Console)
	•	Your OpenAI API Key (insert into environment variable in Cell 1)

3.	Follow Setup Instructions in Notebook
The notebook will guide you through:
	•	Authentication
	•	Required installs
	•	Prompt examples

⸻

📦 Requirements
	•	Python 3.9+
	•	OpenAI Python SDK
	•	LangChain
	•	Google API Client Libraries
	•	TinyDB
	•	dateparser

Install dependencies with:

pip install -r requirements.txt

⚠️ Limitations
	•	This is a prototype notebook: not designed for production use.
	•	Agent flow is currently inefficient (event blocks are created before conflict checking).
	•	Memory is handled via TinyDB (.json) and not yet scalable.
	•	The fallback planner tool may fail due to unresolved UUID logic (not addressed in this version).

⸻

🛡 License

This project is licensed under the MIT License.

