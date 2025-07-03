# 🧠 Intern Job Alerts to Telegram

This project is a no-code/low-code automation built using **n8n**, which fetches the latest job postings related to "intern" or "fresher" roles and sends formatted alerts to a **Telegram channel** daily.

## 📌 Features

- ⏰ **Daily Scheduling** using n8n's built-in trigger.
- 🌐 **Job Data Source**: Fetches listings from [Arbeitnow Job Board API](https://www.arbeitnow.com/api/job-board-api).
- 🔎 **Keyword Filtering**: Filters listings by keywords like `intern` or `fresher`.
- 📤 **Telegram Notification**: Sends structured messages (Title, Company, URL) to a public Telegram channel.

## 🛠️ Workflow Structure

1. **Schedule Trigger** — Executes the workflow once daily.
2. **HTTP Request** — Pulls job data from Arbeitnow API.
3. **Code Node** — Filters listings for `intern` or `fresher` roles.
4. **Message Formatter** — Formats up to 15 jobs into a clean message.
5. **Telegram Sender** — Posts to the configured Telegram channel.

## 📲 Telegram Demo

Join the channel to see live alerts:  
👉 [Join](https://t.me/sentiment_alert_demo)

## 🚀 How to Deploy

1. Self-host n8n via Docker or use n8n Cloud.
2. Import this workflow JSON into n8n.
3. Set up:
   - **Telegram Credentials** via BotFather token.
   - **Telegram Chat ID** (must be admin of the channel).
4. Enable the workflow.

