<img width="919" height="384" alt="image" src="https://github.com/user-attachments/assets/3134a7d2-877d-4b55-8ec1-5fb6b24b269f" />


# 📌 Project: AI Invoice Processor (n8n)

## Description  
This n8n workflow automates the process of extracting and summarizing invoice or receipt data sent via Telegram.  
It uses **OCR** to read the contents of an image, formats the extracted text into a clean summary, and sends it back to the user on Telegram.  
The workflow also uploads the original file to **Google Drive** for storage. It is designed for **Pakistani receipts**, using `Rs.` as the currency format, and includes clear separators for each item in the output.

---

## 🚀 Features

- **Telegram Bot Integration**  
  Triggered when a user sends an image of a receipt or invoice via Telegram.

- **OCR Processing with Tesseract.js**  
  Extracts text from the uploaded image with high accuracy.

- **AI-Powered Text Formatting**  
  Uses **Groq AI (GPT-OSS 20B)** to:  
  - Summarize the receipt content.  
  - Add separators between items to avoid confusion.  
  - Ensure correct Pakistani currency formatting (`Rs.`).

- **Google Drive Backup**  
  Automatically uploads the original image file to a designated Google Drive folder.

- **Instant Telegram Response**  
  Sends a clean, formatted summary back to the user through the same Telegram chat.

---

## 🛠️ Tech Stack & Integrations

- **n8n** – Workflow automation platform  
- **Telegram Bot API** – For sending/receiving messages & images  
- **Tesseract.js** – OCR for text extraction from images  
- **Groq API (GPT-OSS 20B)** – AI text formatting & summarization  
- **Google Drive API** – File storage & organization

---

## 📂 How It Works

1. **User sends a receipt photo** to the Telegram bot.  
2. **n8n retrieves the file** from Telegram.  
3. **Image is uploaded** to Google Drive for backup.  
4. **OCR (Tesseract.js)** extracts the text from the image.  
5. **AI Agent formats the text** into a clean, itemized summary with `Rs.` for all prices.  
6. **Formatted summary is sent back** to the user via Telegram.

---
