# AI-Inbox-Assistant

# 📬 AI Email Automation & Calendar Assistant

An end-to-end email automation system that intelligently reads, analyzes, and responds to emails on your behalf — complete with meeting scheduling, response generation, and activity tracking. Built using **n8n**, **OpenAI**, **Google Calendar**, **Firebase**, and **Google Sheets**.

---

## ✨ Features

- 🔍 **Intent Detection & Categorization**  
  Classifies emails into categories like meeting, sales, project, support, etc., with priority and urgency scoring.

- 🤖 **AI-Powered Email Replies**  
  Auto-generates context-aware, human-like responses based on your tone, personality, and past interactions.

- 📆 **Smart Meeting Scheduling**  
  Extracts times from emails or proposes slots from Google Calendar, then auto-schedules meetings.

- 📊 **Real-Time Analytics & Logging**  
  Tracks engagement, response length, and follow-up suggestions in both Firebase and Google Sheets.

- 📁 **Conversation Context Tracking**  
  Maintains thread-level metadata, conversation stage, and next-suggested actions.

---

## ⚙️ Tech Stack

| Service        | Purpose                                 |
|----------------|-----------------------------------------|
| **n8n**        | Workflow automation                     |
| **OpenAI**     | Email classification & response writing |
| **Google Calendar** | Scheduling and meeting creation   |
| **Gmail API**  | Email parsing and metadata extraction   |
| **Firebase**   | Email engagement logs & analytics       |
| **Google Sheets** | Activity dashboards (optional)      |

---

## 🧠 Workflow Overview

1. **Trigger**: Gmail watch → new email
2. **Extract**: Clean and parse email metadata and body
3. **Analyze**: AI classifies the intent, sentiment, urgency, etc.
4. **Respond**: OpenAI generates the response
5. **Schedule**: Google Calendar slot booking (if needed)
6. **Track**: Data is logged into Firebase + Sheets

---

## 📥 Example Use Cases

- Founders and busy professionals automating their inbox
- Auto-scheduling calls with clients and leads
- Building personal AI assistants that match your tone

---

## 🛠 Setup Instructions

> 📝 Prerequisites:  
> n8n account or self-hosted setup, Gmail & Google Calendar API access, OpenAI API key, Firebase project

1. Clone or import the [emailautomation.json](./emailautomation.json) into n8n.
2. Set up credentials for:
   - Gmail (OAuth2)
   - Google Calendar
   - OpenAI
   - Firebase (Service Account Key)
3. Update personal profile node (`Function - Load Personal Profile`) with your:
   - Name, tone, communication style, working hours
4. Test the flow by sending a sample email.

---

## 📊 Analytics Dashboard (Optional)

- Use the Firebase Realtime Database or Google Sheets to visualize:
  - Emails processed
  - Confidence scores
  - Categories and urgency breakdown
  - Auto-sent vs manually approved responses

---

## 🚀 Roadmap

- [ ] Auto-escalation for critical emails
- [ ] Personalized training via fine-tuned AI responses
- [ ] Slack/Discord notification integrations
- [ ] Admin approval queue for sensitive emails

---

## 🙌 Credits

Built by [Zeeshan Charolia](mailto:charoliazeeshan@gmail.com)  
With ❤️ using n8n, OpenAI, and Google Cloud.

---

## 📄 License

MIT License — open for personal use. Attribution appreciated!
