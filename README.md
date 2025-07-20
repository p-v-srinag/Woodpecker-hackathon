# 🤖 AI-Powered Chatbot – Woodpecker Hackathon Submission

This project is a full-stack **AI chatbot system** developed for the **Woodpecker Hackathon**. It uses **HTML, CSS, JavaScript, PHP, and Python** to provide a seamless user experience for real-time conversation, authentication, and intent-based replies via NLP.

---

## 🌟 Features

- 🧠 AI chatbot that understands user intents
- 🔄 Real-time communication via AJAX
- ☁️ Weather and other external API integrations
- 👥 User login and registration (with PHP + MySQL backend)
- 💬 FAQ and support-based replies using NLP (via `intents.json`)
- 🎨 Frontend with custom landing, login, and chatbot pages
- 🔐 Secure authentication using `login.php` and `users.php`

---

## 🗂️ Project Structure

```
Woodpecker-hackathon/
│
├── chatbot.html         # Chatbot frontend UI
├── intro.html           # Project introduction/landing page
├── login.html           # Login page
├── register.html        # Signup page
├── reachus.html         # Contact form
│
├── styles.css           # General styles
├── landing.css          # Landing page styles
├── script.js            # JS for chat frontend
│
├── server.py            # Python chatbot backend (NLP logic)
├── intents.json         # Intents dataset for chatbot
│
├── login.php            # PHP login logic
├── users.php            # PHP for managing user data
├── config.php           # Database config
│
├── google.png / fb.png / linkedin.png  # Icons
├── chatmodel.png        # Model diagram/image
│
├── README.md
├── package.json / package-lock.json    # (If using Node for frontend assets)
```

---

## 🚀 How to Run This Project

### 🔧 Requirements

- Python 3.7+
- Flask (or any Python HTTP server)
- PHP & MySQL (e.g., XAMPP, LAMP, or WAMP)
- Browser (Chrome/Firefox)
- Optional: Node.js for managing frontend dependencies

---

### 🧠 Step 1: Run the Python Chatbot Server

1. Create a Python virtual environment (optional but recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

2. Install Flask:
   ```bash
   pip install flask
   ```

3. Run the chatbot backend:
   ```bash
   python server.py
   ```

4. It will typically be available at: `http://localhost:5000`

---

### 🌐 Step 2: Set Up PHP Server

1. Install XAMPP/LAMP/WAMP or any other server with PHP + MySQL support.
2. Move the following files to your `htdocs` folder (if using XAMPP):
   - `login.php`, `users.php`, `config.php`, and related `.html` files.

3. Start **Apache** and **MySQL** from XAMPP.

4. Create a MySQL database:
   - Open phpMyAdmin → Create a DB named `chatbot_db` → Add a `users` table (email, password).

5. Configure database credentials in `config.php`.

---

### 💬 Step 3: Use the Chatbot

1. Open `intro.html` in your browser → Navigate to login or register.
2. After login, access `chatbot.html`.
3. Start chatting with the bot — it handles greetings, FAQs, and weather (if integrated).

---

## 🔍 Sample Intents Format (`intents.json`)

```json
{
  "intents": [
    {
      "tag": "greeting",
      "patterns": ["Hi", "Hello", "Hey"],
      "responses": ["Hello there!", "Hi! How can I help you?"]
    },
    {
      "tag": "weather",
      "patterns": ["What's the weather today?", "Tell me the weather"],
      "responses": ["Let me check the weather for you."]
    },
    {
      "tag": "goodbye",
      "patterns": ["Bye", "See you", "Exit"],
      "responses": ["Goodbye!", "Talk to you later!"]
    }
  ]
}
```

---

## 📸 Screenshots

| Login Page | Chat UI |
|------------|---------|
| ![login](login.html) | ![chat](chatmodel.png) |

---

## ✅ Future Improvements

- ✅ Voice input and output using Web Speech API
- ✅ Admin dashboard for intent editing
- ✅ Integration with WhatsApp or Telegram
- ✅ Docker containerization

---

## 🙌 Built With

- HTML, CSS, JavaScript
- PHP + MySQL
- Python (Flask + NLP)
- AJAX for real-time chat
- Developed with ❤️ for the **Woodpecker Hackathon**

---

## 🔗 Clone and Explore

```bash
git clone https://github.com/p-v-srinag/Woodpecker-hackathon.git
cd Woodpecker-hackathon
```

---

⭐️ Star this repo if you found it useful!
