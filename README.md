# AgriVoice 🌾🎙️

**AgriVoice** (`@kisan_viksit_bot`) is an AI-powered, voice-first Telegram assistant designed to help farmers easily access and understand government agricultural schemes. 

Farmers simply send a voice note with their inquiry, and the bot transcribes the speech, consults an LLM for relevant scheme details, and speaks back in clear audio.

---

## 🚀 Features

- **Voice-In, Voice-Out:** Send voice messages directly via Telegram—no typing required.
- **AI-Powered Answers:** Leverages Groq-hosted LLMs for low-latency reasoning and advice on agricultural initiatives.
- **Fast Speech Synthesis:** Generates natural voice responses using `edge-tts`.
- **Farmer-Centric System Prompt:** Grounded in clear, simple language tailored for rural accessibility.

---

## 🛠️ Tech Stack

- **Language:** Python 3.10+
- **Bot Interface:** `python-telegram-bot`
- **LLM / STT Inference:** `groq`
- **Text-to-Speech:** `edge-tts`
- **Environment Management:** `python-dotenv`

---

## 📦 Setup & Installation

### 1. Clone the repository
```bash
git clone [https://github.com/PradeepMittal711/AgriVoice.git](https://github.com/PradeepMittal711/AgriVoice.git)
cd AgriVoice
```

### 2. Set up a virtual environment
```bash
python -m venv .venv
# On Windows:
.venv\Scripts\activate
# On macOS/Linux:
source .venv/bin/activate
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

### 4. Configure environment variables
Copy the example environment file and add your own credentials:
```bash
cp key.env.example key.env
```
Open `key.env` and insert your tokens:
- `TELEGRAM_BOT_TOKEN`: Obtain from [@BotFather](https://t.me/Botfather) on Telegram.
- `GROQ_API_KEY`: Obtain from [Groq Console](https://console.groq.com/).

### 5. Run the bot
```bash
python kisan-voice-bot.py
```
*(Adjust the filename to match your entry point script).*