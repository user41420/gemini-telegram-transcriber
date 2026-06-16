# Gemini Multi-Feature Telegram Bot

A powerful Telegram bot built with Pyrogram and Google Gemini API that supports:

- Audio/Video transcription  
- Image text extraction (OCR)  
- Multilingual output  
- Summarization  
- File or split-message output modes  
- MongoDB user settings storage  
- Multiple bot tokens (multi-bot deployment)

---

## 🚀 Features

### 🎧 Media Transcription
Supports:
- Voice messages  
- Audio files  
- Video files  
- Documents containing media  

Uses Google Gemini 2.5 Flash / Flash-Lite for high-quality transcription.

---

### 🖼️ Image Processing (OCR + Description)
- Extracts text from images accurately  
- If no text is found, generates a detailed image description  

---

### 🌍 Language Support
Supports many languages including:
- English, Arabic, Spanish, French, Russian, German  
- Somali, Swahili, Chinese, Japanese, and more  
- Auto-detect mode available  

---

### 🧠 AI Features
- Smart summarization  
- Clean transcription formatting  
- Multi-speaker separation  
- Grammar correction without changing meaning  
- High-accuracy AI processing via Gemini  

---

### 📦 Output Modes
- Split messages (default)  
- Text file download mode  

---

### 🗄️ Database Support
MongoDB integration for:
- User API keys  
- Language preferences  
- Output mode settings  

---

### 🔐 API Key System
- Each user provides their own Gemini API key  
- Secure per-user processing  
- No shared API usage  

---

## 🛠️ Requirements

- Python 3.10+  
- Telegram Bot Token(s)  
- Google Gemini API Key  
- MongoDB database (optional but recommended)  
- FFmpeg installed  

---

## 🔐 Getting API_ID and API_HASH

1. Go to: https://my.telegram.org  
2. Login with your phone number  
3. Click API development tools  
4. Create a new app  
5. You will receive:
   - API_ID  
   - API_HASH  

⚠️ Keep these private.

---

## 🤖 Getting BOT TOKEN

1. Open Telegram  
2. Search for @BotFather  
3. Run:

/newbot

4. Follow instructions  
5. Copy your BOT TOKEN  

---

## 📦 Installation

```bash
git clone https://github.com/user41420/gemini-telegram-transcriber-bot.git
cd gemini-telegram-transcriber-bot
pip install -r requirements.txt


⸻

⚙️ Environment Variables

Create a .env file or set variables manually:

API_ID=123456
API_HASH=your_api_hash
BOT_TOKENS=bot_token1,bot_token2
MONGO_URL=mongodb+srv://your_mongo_url
MAX_UPLOAD_MB=1000
DOWNLOADS_DIR=./downloads


⸻

▶️ Run Bot

python main.py


⸻

📁 Project Structure

.
├── main.py
├── downloads/
├── requirements.txt
└── README.md


⸻

🔑 How It Works
 1. User sends /start
 2. User provides Gemini API key
 3. User sends audio/image/video
 4. Bot processes via Gemini API
 5. Returns:
 • Transcript / OCR text / summary
 • File or split message output

⸻

📌 Commands

Command Description
/start Start bot
/help Show help
/lang Select language
/mode Choose output mode


⸻

⚠️ Notes
 • Large files are processed temporarily
 • Requires FFmpeg for audio conversion
 • API key required per user
 • Supports multi-bot deployment

⸻

👨‍💻 Tech Stack
 • Python
 • Pyrogram
 • Google Gemini API
 • MongoDB (Motor)
 • FFmpeg
 • AsyncIO

⸻

📜 License

MIT License

⸻

💡 Author

Built with advanced AI integration for Telegram automation and transcription systems.

.
