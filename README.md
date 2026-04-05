# 📝 Responsive AI Notepad

A **modern, responsive web-based notepad** with rich text formatting, **AI-powered autocorrect**, and **word suggestions**.
This project enhances the traditional note-taking experience using intelligent features and a clean UI.

---

## 🚀 Features

✨ **Rich Text Formatting**

* Bold, Italic, Underline options
* Dynamic toolbar with active state highlighting

🤖 **AI Autocorrect**

* Automatically corrects the last typed word
* Uses a local AI API (`gemma2:2b` model)

💡 **Word Suggestions**

* Suggests the next word while typing
* Helps improve writing speed and accuracy

💾 **Auto Save (Local Storage)**

* Saves notes in browser storage
* Loads previous notes automatically on reload

📱 **Responsive Design**

* Works seamlessly on desktop and mobile devices

---

## 🛠️ Tech Stack

* **HTML5**
* **CSS3 (Responsive UI)**
* **JavaScript (Vanilla JS)**
* **LocalStorage API**
* AI API (Local server - Ollama / LLM endpoint)

---

## 📂 Project Structure

```
project-folder/
│── index.html   # Main application file
```

---

## ⚙️ How It Works

1. User types inside a **contenteditable notepad**
2. On pressing **spacebar**:

   * Autocorrect fixes the last word (if enabled)
   * Suggestion API predicts the next word (if enabled)
3. Notes are saved using **localStorage**
4. Toolbar buttons apply formatting using `execCommand`

---

## ▶️ How to Run the Project

### ✅ Method: Direct Open

```bash
start index.html
```

---

## 🔌 API Configuration

This project uses a **local AI API endpoint**:

```
http://localhost:11434/api/chat
```

### Requirements:

* Install and run Ollama
* Pull model:

```bash
ollama run gemma2:2b
```

---

## 🧠 AI Prompt Behavior

### Autocorrect:

* Returns only the corrected word
* No extra text

### Suggestion:

* Predicts the next word
* Returns only one word

---

## 📸 UI Overview

* Clean card-based notepad layout
* Toolbar with toggle buttons
* Live status showing last saved time

---

## ⚠️ Limitations

* Uses `document.execCommand()` (deprecated but still supported)
* Requires local AI server running
* No backend database (only browser storage)

---

## 🔮 Future Improvements

* Replace `execCommand` with modern APIs
* Add cloud sync (Firebase / backend)
* Add multi-note support
* Improve AI suggestions with better context models
* Add dark mode 🌙


✅ Convert this into a **portfolio-ready GitHub project**
✅ Add **badges (stars, license, tech stack)**
