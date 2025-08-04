# lab-request-workflow-bot
A chatbot-based request system for labs using N8n workflow automation, integrated with Google Sheets and Gmail for tracking and notifications to supervisors.
This project automates the process of collecting lab agent requests through a chatbot interface. The chatbot is deployed on Hugging Face or Tidio and connected to an N8n automation workflow that stores data in a Google Sheet and sends email alerts.

Features

- Webhook-based chatbot integration
- Field conversion and validation
- Auto-log to Google Spreadsheet
- Sends email notifications with request details

Tech Stack

- Tidio / Hugging Face – Chatbot frontend
- N8n – Automation workflow engine
- Google Sheets API – For tracking requests
- Gmail API – For sending email alerts
- Ngrok – Local tunnel to expose webhook

Files

- `n8n-workflow-lab-agent.json` – Exported N8n workflow
- `README.md` – This file

---

Workflow

1. User interacts with chatbot(gives information about what reagent or any other lab equipment they want).
2. Webhook in N8n catches data
3. Data is cleaned and fields are converted
4. Request is added to Google Sheet
5. Email is sent to the lab manager or supervisor.

Here is what the chatbot looks like:
(2nd chatbot.png) and (chatbot ss.png) 

Chat with my chatbot here on huggingface:
https://noor123456-my-first-chatbot.hf.space/

