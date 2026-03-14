# 🤖 AI Text Analyzer

A Python CLI tool that reads any `.txt` file and uses **Groq AI** to automatically extract a summary, sentiment, and key topics. Built as part of my AI Engineer learning journey.

---

## 🎯 What It Does

Give it any text file and it returns:

- 📝 **Summary** — one paragraph overview
- 😊 **Sentiment** — positive, negative, or neutral
- 🏷️ **Key Topics** — main themes extracted from the text

---

## 🖥️ Demo Output

```
📝 Summary:   AI is transforming the world with major investments
              from Google, Microsoft and OpenAI. Python has become
              the most popular language for AI development.

😊 Sentiment: positive

🏷️  Topics:   ['Artificial Intelligence', 'Python',
               'Machine Learning', 'Future of AI']
```

---

## 🛠️ Built With

| Tool | Purpose |
|------|---------|
| Python 3 | Core language |
| Groq API | LLaMA AI model |
| JSON | Structured output parsing |
| dotenv | Secure API key management |
| Prompt Engineering | Control AI output format |

---

## 🚀 How To Run

### 1. Clone the repository
```bash
git clone https://github.com/pathananas212/ai-text-analyzer.git
cd ai-text-analyzer
```

### 2. Install dependencies
```bash
pip install groq python-dotenv
```

### 3. Set up your API key
Create a `.env` file:
```
GROQ_API_KEY=your_groq_api_key_here
```
Get a free key at [console.groq.com](https://console.groq.com)

### 4. Add your text
Edit `article.txt` with any text you want to analyze.

### 5. Run the analyzer
```bash
python ai_text_analyzer.py
```

---

## 📦 Project Structure

```
ai-text-analyzer/
│
├── ai_text_analyzer.py  # Main script
├── article.txt          # Sample input file
├── .env                 # API key (never uploaded!)
├── .gitignore           # Ignores .env and secrets
└── README.md            # Project documentation
```

---

## 🧠 How It Works

```
article.txt
    ↓  open() reads the file
text variable
    ↓  f-string builds the prompt
Groq API receives prompt + text
    ↓  LLaMA AI analyzes content
Returns structured JSON response
    ↓  json.loads() parses it
Clean formatted output displayed
```

---

## 💡 Skills Learned

- ✅ File handling — `open()`, `read()`, file modes
- ✅ JSON parsing — `json.loads()`, `json.dumps()`
- ✅ Prompt engineering — controlling AI output format
- ✅ API integration — Groq LLaMA API
- ✅ Error handling — `try/except`
- ✅ Secure secrets — `.env` + `python-dotenv`
- ✅ AI roles — `system`, `user`, `assistant`

---

## 🗺️ Future Upgrades

- [ ] Analyze multiple files at once
- [ ] Save results to JSON file
- [ ] Add web interface with Flask
- [ ] Support PDF files
- [ ] Compare sentiment across multiple articles

---

## 👨‍💻 Author

**Mohammed Anas Khan Pathan**
- GitHub: [@pathananas212](https://github.com/pathananas212)
- CS Graduate Student @ University of Texas Arlington
- Building toward a career in AI Engineering 🚀

---

## 📚 Part Of My AI Engineer Journey

```
✅ Project 1 — File Organizer Bot
✅ Project 2 — AI Chatbot
✅ Project 3 — Stock Price Tracker
✅ Project 4 — AI Text Analyzer     ← YOU ARE HERE
⏳ Project 5 — GitHub AI Tracker
⏳ Project 6 — RAG Document Search
⏳ Project 7 — AI Workflow Agent
```
