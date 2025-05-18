# Welcome Email Generator (n8n Automation)

This n8n workflow automates generating personalized welcome emails using the LLaMA-3 model via OpenRouter API, based on Google Sheet input.

---

## 🛠 How to Import the Workflow

1. Open n8n (self-hosted or cloud).
2. Click "Import Workflow".
3. Upload `welcome-email-generator.json`.

---

## 🔐 Where to Add Credentials

### Google Sheets:
- Go to **Credentials → Google Sheets OAuth2 API**.
- Connect your Google account and select the created sheet.

### OpenRouter API (for LLaMA-3):
- Go to **Credentials → HTTP Basic Auth or Header Auth**.
- Create a new HTTP Auth credential named `OpenRouter API`.
- Under headers, add:
  - Key: `Authorization`
  - Value: `Bearer YOUR_API_KEY_HERE`

---

## ▶ How to Run / Test

1. Replace the `YOUR_API_KEY_HERE` with your actual OpenRouter API key.
2. Make sure your Google Sheet contains at least 5 rows with:
   - Unique `email`, `name`, `status` = `not-send`, and empty `content`.
3. Execute the workflow manually or schedule it.
4. Check the Google Sheet — email content will be generated and inserted, and `status` will be updated to `send`.

---

## 🌐 OpenRouter API Endpoint Used

