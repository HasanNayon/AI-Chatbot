# AI Chatbot with LangChain and Streamlit


🔗 **Try the Live Chatbot Here:** [AI Gemma Chatbot](https://aigemmachatbot.streamlit.app/)

## The project UI

[![AI Chatbot](https://raw.githubusercontent.com/HasanNayon/AI-Chatbot/main/Screenshot%202025-03-28%20233507.png)](https://aigemmachatbot.streamlit.app/)

## 📌 Project Overview

This project is an AI-powered chatbot built using LangChain and Streamlit. The chatbot leverages the Groq API for generating AI responses and includes conversation memory to maintain context throughout interactions. The interface is designed using Streamlit, making it accessible via a simple web application.

## 🛠️ Features

- **Conversational Memory:** Uses `ConversationBufferMemory` to remember chat history.
- **Customizable AI Responses:** Adjust AI response creativity using a temperature slider.
- **User-Friendly Interface:** Built with Streamlit for easy interaction.
- **Lightweight and Fast:** Uses ChatGroq for efficient response generation.

## 🚀 Installation & Setup

### Prerequisites

Ensure you have Python 3.8+ installed on your system.

### 1️⃣ Clone the Repository

```sh
git clone https://github.com/your-repo/ai-chatbot.git
cd ai-chatbot
```

### 2️⃣ Install Required Packages

Create a virtual environment (optional but recommended) and install dependencies:

```sh
pip install -r requirements.txt
```

### 3️⃣ Set Up API Key

Add your Groq API Key to the environment variables:

```sh
export GROQ_API_KEY='your-api-key-here'
```

Or set it inside `model.py`:

```python
import os
os.environ["GROQ_API_KEY"] = "your-api-key-here"
```

### 4️⃣ Run the Application

```sh
streamlit run app.py
```

This will launch the chatbot in your browser.

## 📂 Project Structure

```
├── model.py       # AI model and response logic
├── app.py         # Streamlit UI and chatbot interface
├── requirements.txt  # Required dependencies
├── README.md      # Project documentation
```

## 🎛️ Customization

- Modify the AI response temperature in `app.py` (default: 0.7):

```python
temperature = st.sidebar.slider("Response Creativity (Temperature)", 0.0, 1.0, 0.7)
```

- Adjust the prompt template in `model.py` to change AI behavior.

## 🔧 Troubleshooting

If you encounter any issues:

- Ensure all dependencies are installed:
  ```sh
  pip install -r requirements.txt
  ```
- Check if your API Key is correctly set.
- Restart the app:
  ```sh
  streamlit run app.py
  ```

## 💡 Acknowledgments

- [LangChain](https://www.langchain.com/)
- [Streamlit](https://streamlit.io/)
- [Groq API](https://groq.com/)
