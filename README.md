# 🤖 AI Administrative Assistant

An AI-powered administrative expense automation system built with n8n.

This workflow allows users to submit expense transactions through Telegram using either text messages or receipt images. The system automatically extracts, validates, and stores the transaction data.

## ✨ Features

- 💬 Text-based expense input via Telegram
- 🧾 Receipt image processing
- 🔎 OCR text extraction
- 🤖 AI-powered transaction parsing
- ✅ Transaction validation
- 🆔 Automatic transaction ID generation
- ☁️ Receipt upload to Google Drive
- 📊 Automatic recording to Google Sheets
- 🔗 Receipt link generation
- 📩 Automatic confirmation via Telegram

## 🔄 Workflow

```text
Telegram
   │
   ├── Text ──────→ AI Parser ──→ Validation
   │
   └── Receipt ───→ OCR ──→ AI Parser ──→ Validation
                                      │
                                      ↓
                              Transaction ID
                                      │
                                      ↓
                                    Merge
                                      │
                                      ↓
                              Google Sheets
                                      │
                                      ↓
                              Telegram Reply
```

## 🛠️ Tech Stack
n8n
Telegram Bot API
Groq
Llama 3.3 70B
OCR.Space
Google Drive
Google Sheets
JavaScript
🧠 Example
Input

Beli printer untuk divisi HR sebesar 1,5 juta.

AI Output
{
  "tanggal": "14 August 2026",
  "kategori": "Pembelian",
  "deskripsi": "Pembelian printer",
  "nominal": 1500000,
  "divisi": "HR"
}
🎯 Purpose

This project demonstrates how AI and workflow automation can reduce repetitive administrative data entry.

Instead of manually transferring transaction information from messages or receipts into spreadsheets, the workflow automates the extraction, validation, storage, and confirmation process.

🔐 Security

Credentials, API keys, and personal resource IDs have been removed from the public workflow.

Users must configure their own credentials before running the workflow.

📁 Repository Structure
ai-administrative-assistant/
│
├── workflow/
│   └── ai-administrative-assistant.json
│
├── screenshots/
│   └── ...
│
└── README.md
📌 Project Status

Prototype / Portfolio Project

Built to demonstrate practical experience in:

AI Workflow Automation
LLM Integration
Prompt Engineering
OCR Processing
API Integration
JavaScript
Data Automation
👤 Author

Muhammad Zaki

GitHub: MuhammadZaki1709
