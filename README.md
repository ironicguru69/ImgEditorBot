# 🖼️ Telegram Image Editor Bot

Ek powerful Telegram bot jo images edit karta hai — Rounded Corners, Background Remove, aur Sticker banata hai!

---

## ✨ Features

| Feature | Description |
|---|---|
| ✂️ **Crop & Round** | Image crop + rounded corners (3 sizes) |
| 🪄 **BG Remove** | AI se background remove |
| 🎭 **Sticker** | Telegram WebP sticker banana |

---

## 🚀 Railway pe Deploy Kaise Karein

### Step 1 — Bot Token Lo

1. Telegram pe **@BotFather** ko message karo
2. `/newbot` likho
3. Naam aur username do
4. **Token copy kar lo** (aise dikhta hai: `7123456789:AAH...`)

---

### Step 2 — Railway Account Banao

1. **[railway.app](https://railway.app)** pe jao
2. GitHub se login karo (free hai)

---

### Step 3 — GitHub pe Code Upload Karo

1. **[github.com](https://github.com)** pe ek naya repository banao (e.g. `tg-image-bot`)
2. In files ko upload karo:
   - `bot.py`
   - `requirements.txt`
   - `Procfile`
   - `railway.toml`

---

### Step 4 — Railway pe Deploy Karo

1. Railway dashboard mein **"New Project"** click karo
2. **"Deploy from GitHub repo"** choose karo
3. Apna repo select karo
4. Deploy shuru ho jayega ✅

---

### Step 5 — BOT_TOKEN Set Karo

1. Railway project mein **"Variables"** tab pe jao
2. **"New Variable"** click karo
3. Key: `BOT_TOKEN`
4. Value: apna token paste karo (jo BotFather se mila tha)
5. **Save** karo — bot automatically restart ho jayega

---

## 💬 Bot Use Kaise Karein

```
1. Bot ko Telegram pe dhundo
2. /start karo
3. Koi bhi photo bhejo
4. Button press karo:
   ✂️ Crop & Round → radius choose karo
   🪄 BG Remove → background hat jayegi
   🎭 Sticker → WebP file milegi
```

---

## 🛠️ Local PC pe Run Karna Hai?

```bash
# Dependencies install karo
pip install -r requirements.txt

# Token set karo
export BOT_TOKEN="your_token_here"   # Linux/Mac
set BOT_TOKEN=your_token_here        # Windows

# Bot run karo
python bot.py
```

---

## 📦 Dependencies

- `python-telegram-bot` — Telegram API
- `Pillow` — Image processing
- `rembg` — AI background removal
- `onnxruntime` — rembg ke liye

---

## ❓ Common Issues

| Problem | Solution |
|---|---|
| Bot respond nahi kar raha | BOT_TOKEN sahi set karo |
| BG Remove kaam nahi karta | `rembg` install check karo |
| Railway deploy fail | `requirements.txt` check karo |

---

## 📸 Bot Preview

```
User: [photo bheja]
Bot: ✅ Photo receive ho gayi! Ab feature choose karo 👇
     [✂️ Crop & Round] [🪄 BG Remove]
     [🎭 Sticker (WebP)]
     [ℹ️ Help]
```

Made with ❤️ by Gulshan
