# 🧨 Mines Bot

Telegram bot for the **1WIN Mines** game that provides "predictions" for moves/codes.
The bot supports **multiple languages** (Russian, English, Hindi, Spanish, Azerbaijani, Portuguese/Brazilian, Turkish, Arabic, Uzbek).

## ⚡️ Features

* 🎰 Generates signals for the *Mines* game on 1WIN.
* 🌍 Multi-language support (9+ languages).
* 🤖 Built on the asynchronous framework **[Aiogram 3.x](https://docs.aiogram.dev/)**.
* 💾 Uses **SQLite** (via `aiosqlite`) for user data storage.
* 🔑 Subscription check before accessing the bot.
* 📝 Registration and detailed instructions inside the bot.
* 🛠 Custom promo code (**PROMO**) support.

## 📂 Project Structure

```
minesbot-main/
│── main.py            # Entry point:contentReference[oaicite:0]{index=0}
│── config.py          # Config (token, channel, promo, etc.):contentReference[oaicite:1]{index=1}
│── requirements.txt   # Dependencies:contentReference[oaicite:2]{index=2}
│── handlers/          # Client/admin handlers
│── database/          # Database logic (SQLite)
│── other/             # Filters and utilities
│── Procfile           # For deployment (Heroku, etc.)
│── start.bat          # Quick start script for Windows
│── install.bat        # Install dependencies script
│── hel.jpg / hello.jpg # Images
```

## 🛠 Installation & Run

### 1. Clone the repository

```bash
git clone https://github.com/USERNAME/mines-bot.git
cd mines-bot
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Configure the bot

Edit **config.py** with your own data:

```python
BOT_TOKEN = "YOUR_BOT_TOKEN"
CHANNEL_URL = "https://t.me/your_channel"
CHANNEL_ID = "-100XXXXXXXXXXXX"
VERIF_CHANNEL_ID = "-100YYYYYYYYYYYY"
ADMIN_ID = 123456789
PROMO = "YOUR_PROMO"
```

### 4. Run the bot

```bash
python main.py
```

Or use the quick start script on Windows:

```bash
start.bat
```

## 📦 Deployment

This project can be deployed to:

* 🟣 **Heroku** (via Procfile)
* 🐳 Docker (optional)
* Any VPS/server with Python 3.10+

## ⚠️ Disclaimer

> This bot was created for educational purposes only.
> Use with gambling services is at your own risk.
