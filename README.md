# WhatsApp CV Bot

A WhatsApp bot built with **Flask**, **Twilio**, and **Google Sheets** that automatically parses resumes (PDF, Word, or image), extracts candidate details (Name, Email, Phone) using **Google Gemini AI**, and stores them in Google Sheets.

---

## 🌟 Key Features

- **WhatsApp-first:** Candidates send resumes directly to your WhatsApp number.
- **Smart Parsing:** Reads PDFs, Word docs, and even images (OCR with Tesseract).
- **AI Extraction:** Uses **Google Gemini AI** to pull Name, Email, and Phone accurately.
- **Instant Storage:** Adds extracted data to Google Sheets seamlessly.
- **Real-Time Dashboard:** Live UI updates using Server-Sent Events (SSE) to monitor submissions.
- **Fallback Safety:** If phone numbers are missing, defaults to WhatsApp number.

---

## 🛠 Tech Stack

| Layer | Technology |
|-------|------------|
| Backend | Python, Flask |
| Messaging | Twilio WhatsApp API |
| AI Parsing | Google Gemini AI |
| File Parsing | PyPDF2, python-docx, pytesseract, Pillow |
| Storage | Google Sheets (gspread) |
| DevOps | python-dotenv, Render/Gunicorn deployment |

---

## 🚀 How It Works

1. Candidate sends a resume to your **Twilio WhatsApp number**.
2. Bot downloads the file and determines its type.
3. Text is extracted (OCR for images, text extraction for PDF/Word).
4. **Gemini AI** parses the text and structures candidate details.
5. Data is appended to **Google Sheets** and visible in the live dashboard.
6. Candidate receives a WhatsApp confirmation ✅.

---

