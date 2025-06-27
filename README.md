💬 WSP ChatBot

A simple AI-powered chatbot web application built using **Flask**, **HTML/CSS/JS**, and integrated with the **OpenRouter AI API** to generate intelligent responses.

---

## 🚀 Features

- 🧠 AI Chat powered by the `deepseek/deepseek-r1:free` model via OpenRouter API  
- 🎨 Clean and responsive Bootstrap-based UI  
- 🔁 Smooth interaction between user and AI in a conversational interface  
- 🛠️ Lightweight backend using Python Flask  
- 📡 Asynchronous communication using `fetch()` for fast responses  
- 🧪 Error handling for API failures  

---

## 📁 Project Structure

```
├── app.py              # Flask backend server
├── templates/
│   └── index.html      # Frontend chat interface
```

---


## 🔧 Installation & Setup

### 🖥️ Requirements

- Python 3.7+
- `Flask`
- Internet connection (for external API requests)

### 🔌 Installation

1. **Clone the repository**

2. **Create a virtual environment (optional but recommended)**

```bash
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
```

3. **Install dependencies**

```bash
pip install flask requests
```

4. **Set up your OpenRouter API key**

Update the `API_KEY` variable in `app.py`:
```python
API_KEY = "your-api-key"
```

5. **Run the Flask app**

```bash
python app.py
```

6. **Access the chatbot**

Open your browser and navigate to `http://127.0.0.1:5000/`

---

## 🌐 How It Works

### Frontend (`index.html`)

- Built with Bootstrap 4 for styling.
- Provides a chat interface with user input.
- Sends messages via JavaScript `fetch()` to the Flask backend.
- Appends responses from the AI to the conversation view.

### Backend (`app.py`)

- Handles `/` route to render the chat UI.
- Handles `/chat` POST request for incoming user messages.
- Sends user input to OpenRouter API with proper headers and payload.
- Extracts and returns the AI-generated response.

---

## 🧠 AI Model Info

- Model used: `deepseek` 
- API endpoint: `https://openrouter.ai/api/v1/chat/completions`

> 🔐 **Make sure your API key is valid and kept secure.**  

---

## 💡 Example Usage

```
You: What is the capital of France?
Bot: The capital of France is Paris.
```

## 🙌 Acknowledgements

- [Flask](https://flask.palletsprojects.com/)
- [Bootstrap](https://getbootstrap.com/)
- [OpenRouter](https://openrouter.ai/)
- [DeepSeek](https://www.deepseek.com/)

---

## 👤 Author

**Dravya Gangwal**  
📧 [dravyagangwal25@gmail.com]
