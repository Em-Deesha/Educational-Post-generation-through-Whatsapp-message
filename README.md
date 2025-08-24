# Educational-Post-generation-through-Whatsapp-message

# Automated Educational Post Creator (WhatsApp → Gemini → Google Sheets)

## 📌 Overview
This workflow automates the process of creating **educational posts** using **WhatsApp input**, **Google Gemini AI**, **HTML image generation**, and **Google Sheets integration**.  
The goal is to make social media content creation **fast, structured, and automated**.

---

## ✅ Features
- **WhatsApp Trigger** → Capture user topic from WhatsApp message.
- **AI Content Generation (Gemini)** → Generate educational post content with multiple options.
- **Image Generation (HCTI API)** → Convert HTML-styled content into a visually appealing dark theme image.
- **Caption Generation (Gemini)** → Create Instagram-friendly captions with trending hashtags.
- **Google Sheets Integration** → Store Topic, Image URL, Caption, and Status (Pending/Posted) for easy tracking.

---

## 🛠 Workflow Components
### 1. Post Creation (First Branch)
- WhatsApp message is captured.
- Gemini generates 3 content options.
- User selects an option.
- HTML + CSS styling applied.
- Image generated via **HCTI API**.

### 2. Caption Generation (Second Branch)
- Gemini creates short, engaging captions.
- Adds 5 trending hashtags.
- Captions are educational and under 100 characters.

### 3. Google Sheets Logging
- Append new row with:
  - **Topic**
  - **Image URL**
  - **Caption**
  - **Status** = `Pending`

---

## 📂 Tech Stack
- **n8n** → Workflow automation tool.
- **Google Gemini API** → AI content & caption generation.
- **HCTI.io API** → HTML to image conversion.
- **Google Sheets API** → Data storage.
- **WhatsApp API** → Topic input from user.

---

## 🔗 Data Flow


---

## ⚙ Setup Instructions
1. Clone this repo.
2. Install and run **n8n** locally or on a server.
3. Add credentials for:
   - **WhatsApp API**
   - **Google Gemini**
   - **Google Sheets**
   - **HCTI.io**
4. Import the workflow into n8n.
5. Update your Google Sheet with columns:
Topic | Image URL | Caption | Status
6. Execute the workflow.
