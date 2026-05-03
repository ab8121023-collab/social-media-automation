# 🤖 Social Media Auto Poster

AI-powered social media automation that automatically generates and posts content to Facebook and Instagram.

---

## ✨ Features

- 🧠 AI caption generation using Groq (Llama 3.3)
- 🖼️ Auto image fetching from Pexels API
- 📘 Auto posting to Facebook Page
- 📸 Auto posting to Instagram Business Account
- 📊 Google Sheets for post management
- 📱 Telegram alerts for errors
- ⏰ Scheduled daily posting at 7 AM

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| n8n | Workflow Automation |
| Groq AI - Llama 3.3 | Caption Generation |
| Pexels API | Image Fetching |
| Meta Graph API | Facebook & Instagram Posting |
| Google Sheets | Post Management |
| Telegram Bot | Error Notifications |

---

## 📋 How It Works
Google Sheet (pending posts)
↓
AI generates caption + hashtags
↓
Pexels fetches relevant image
↓
Posts to Facebook + Instagram
↓
Updates Sheet status (done/failed)
↓
Telegram alert if error

---

## 📊 Google Sheet Structure

| Column | Description |
|--------|-------------|
| ID | Unique post ID |
| Topic | Post topic |
| keywords | Image search keywords |
| Status | pending / done / failed |
| Platform | Facebook / Instagram |
| Post_Date | Scheduled date |
| Post_Time | Scheduled time |

---

## 🚀 Setup Guide

### 1. Prerequisites
- n8n installed (local or cloud)
- Meta Developer Account
- Groq API Key
- Pexels API Key
- Telegram Bot

### 2. Import Workflow

Open n8n
Click "..." menu
Click "Import from file"
Select workflow.json
Add your credentials


### 3. Required Credentials
META_SYSTEM_USER_TOKEN = your_token
GROQ_API_KEY = your_key
PEXELS_API_KEY = your_key
TELEGRAM_BOT_TOKEN = your_token
TELEGRAM_CHAT_ID = your_chat_id

### 4. Meta App Permissions Required

- pages_manage_posts
- pages_read_engagement
- instagram_basic
- instagram_content_publish

---

## 📁 Project Structure
social-media-automation/
├── workflow.json              # n8n workflow file
├── credentials-template.txt  # Credentials template
└── README.md                 # Documentation

---

## ⚠️ Security Notes

- Never commit real API tokens
- Use credentials-template.txt as reference only
- Keep Meta System User Token secure

---

## 👤 Author

**Ali Raza** — Ai Spark Agency

🌐 [Facebook](https://www.facebook.com/aispark.agency)

---

## 📄 License

MIT License — Free to use and modify
