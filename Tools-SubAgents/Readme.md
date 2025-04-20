# 🤖 AI Agents – Personal Assistant System with n8n

A modular, configuration-driven personal assistant framework built using **n8n**, inspired by real-time voice AI like **Amazon Nova Sonic** https://bit.ly/4jLQxsx . This system uses a central workflow to coordinate multiple specialized AI agents designed for real-world automation and productivity.
---

## 🧠 Overview
![Screenshot 2025-04-20 193143](https://github.com/user-attachments/assets/1d80aa14-1050-4223-87a6-12113779e940)
This project focuses on orchestrating task-specific agents through a central workflow (`Main_workFlow.json`). Each sub-agent is defined using a JSON config and performs a specific function (e.g., email handling, calendar management, fitness tracking). Agents can be easily added, modified, or removed for flexibility and scalability.

---

## 📂 Project Structure

.
├── Main_workFlow.json                 # Central orchestration workflow
├── README.md                         # Project overview and usage guide
└── Tools-SubAgents/
    ├── Email_agent.json              # Handles email-related tasks
    ├── calendar_event_agent.json     # Manages calendar events
    ├── fitness_Agent.json            # Integrates with Fitbit for fitness data
    ├── personal_data_RAGagent.json   # Retrieves and processes personal data (RAG-based)
    └── research_Agent.json           # Conducts online research and summarization


---

## ⚙️ Key Features

- 🧩 **Pluggable Sub-Agents**: Each agent has a defined role and can be reused or replaced as needed.
- 📊 **Fitness Tracking**: The `fitness_Agent.json` uses the **Fitbit API** to incorporate real-time health and activity data.
- 🔁 **Dynamic Orchestration**: `Main_workFlow.json` determines how and when agents are invoked.
- 🌱 **Scalable & Extensible**: Add new agents by dropping a new JSON config into `Tools-SubAgents`.

---

## 🛠 Technologies Used

- [n8n](https://n8n.io/) – Visual workflow automation
- REST APIs – For external integrations (e.g., email, calendar, Fitbit, etc.)
- (Optional) RAG techniques – For contextual personal data retrieval
- Elevenlabs

---

## 🚀 Getting Started

1. Clone the repo:
   ```bash
   git clone https://github.com/Smith-S-S/Ai-Agents.git
