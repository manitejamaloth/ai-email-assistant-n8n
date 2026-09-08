# AI Email Assistant — Inbox Automation with n8n

An automated n8n workflow that scans a user's inbox every morning, uses AI to summarize and triage emails, drafts replies, and sends a daily digest via Telegram — with one-tap approval to auto-send replies.

## 🎯 Problem

Manually checking, reading, and responding to emails every day is time-consuming — especially separating what needs a reply from what doesn't.

## ⚙️ How It Works

1. **Trigger**: Workflow runs automatically every morning at 8 AM.
2. **Scan**: Connects to the inbox and pulls new emails.
3. **AI Summarization**: An LLM summarizes each email and determines whether a reply is needed.
4. **Draft Generation**: If a reply is required, AI drafts a response and saves it directly as a draft in the inbox.
5. **Telegram Notification**: Sends a summary of the day's emails to the user via Telegram.
6. **One-Tap Approval**: If the user approves via Telegram, the AI-drafted reply is automatically sent to the original sender.

## 🛠️ Tools Used

- **n8n** — workflow orchestration
- **LLM API** (OpenAI / Gemini / Claude) — email summarization and reply generation
- **Telegram Bot API** — notifications and approval flow
- **Email/IMAP integration** — inbox access

## 📸 Workflow Screenshot

![Workflow Screenshot](https://github.com/manitejamaloth/ai-email-assistant-n8n/blob/454642c38d41bd5cff318ddbabdc9254e00cfc49/Screenshot%202026-09-08%20213014.png)

## 📄 Workflow Export

Full workflow JSON available in this repo — see `[workflow.json](https://github.com/manitejamaloth/ai-email-assistant-n8n/blob/b83227b54bd22dfe3e732025a9873933fde9c362/AI-Powered%20Email%20Asst.json)`

## 💡 Impact

Reduces manual inbox management time significantly by automating triage and response drafting, while keeping a human-in-the-loop for final approval.
