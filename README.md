# Welcome Email Generator – n8n Automation

This project is an n8n-based automation workflow that generates personalized welcome emails using AI and updates a Google Sheet with the email content and status.

## ✨ Features

- Reads user data from a connected Google Sheet.
- Uses OpenAI to generate a personalized welcome email for each contact.
- Writes the email content back to the sheet.
- Updates the status to avoid duplicate processing.
- Clean and efficient logic using just 3–4 nodes.
- Easily extendable for logging, notifications, or integrations.

## 📋 Tech Stack

- **n8n** (Low-code automation)
- **Google Sheets API**
- **OpenAI Chat Model** (via AI Agent node)
- **Node-based workflow**

## 🚀 Setup & Usage

### 1. Clone this repository

```bash
git clone https://github.com/your-username/welcome-email-automation.git
cd welcome-email-automation
