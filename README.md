# 🤖 WhatsApp PDF Bot

A simple WhatsApp bot that sends PDF files automatically when users request them 📄✨

---

## 🚀 Features

- 📚 **Auto PDF List** – Users can get a full list of available PDFs  
- 🔢 **Number-Based Selection** – Just reply with a number to receive a file  
- ⚡ **Fast Response** – Instantly sends requested PDFs  
- 🛠️ **Error Handling** – Handles missing files & issues smoothly  

---

## 📦 Setup Guide

### 1️⃣ Install Dependencies
```bash
npm install whatsapp-web.js qrcode-terminal
```

### 2️⃣ Add Your PDF Files

Create a folder named `files/` and add your PDFs:

```
files/
├── Lesson 03.pdf
├── Lesson 04.pdf
├── Lesson 05.pdf
├── Lesson 10.pdf
├── Lesson 08.pdf
└── Teachers Guide.pdf
```

### 3️⃣ Run the Bot
```bash
node whatsapp-pdf-bot.js
```

### 4️⃣ Connect WhatsApp

- A QR code will appear in your terminal 📱  
- Scan it using WhatsApp  
- Bot will be ready ✅  

---

## 💡 How It Works

### 📥 Step 1 – Request List
User sends:
```
pdf
```
or
```
files
```

### 📤 Step 2 – Bot Reply
```
📚 Available PDF Files:

1. Lesson 03.pdf
2. Lesson 04.pdf
3. Lesson 05.pdf
4. Lesson 10.pdf
5. Lesson 08.pdf
6. Teachers Guide.pdf

👉 Reply with the number to get the file.
```

### 📨 Step 3 – Get File
User replies:
```
5
```

Bot sends:
```
Lesson 08.pdf 📄
```

---

## 🗂️ Project Structure

```
├── whatsapp-pdf-bot.js
├── files/
│   ├── Lesson 03.pdf
│   ├── Lesson 04.pdf
│   ├── Lesson 05.pdf
│   ├── Lesson 10.pdf
│   ├── Lesson 08.pdf
│   └── Teachers Guide.pdf
└── README.md
```

---

## ⚙️ Customize PDFs

Edit your file list inside `whatsapp-pdf-bot.js`:

```javascript
const pdfs = {
  "1": "files/Lesson 03.pdf",
  "2": "files/Lesson 04.pdf",
  "3": "files/Lesson 05.pdf",
  "4": "files/Lesson 10.pdf",
  "5": "files/Lesson 08.pdf",
  "6": "files/Teachers Guide.pdf",
  "7": "files/New File.pdf"
};
```

---

## 🧪 Tips

- ✔ File names must match exactly  
- ✔ Keep all PDFs inside `files/` folder  
- ✔ Ensure stable internet connection  

---

## ⭐ Simple & Powerful

Perfect for:
- Sharing lessons 📘  
- Distributing notes 📝  
- Automating file delivery ⚡  
