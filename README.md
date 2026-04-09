# 💳 (CSV Agent) Smart Banking Transaction Analysis with AI

🚀 This project analyzes banking transaction data to uncover spending patterns, detect anomalies, and generate AI-powered financial insights using **LangChain + Groq LLM**.

---

## 🎥 Project Demo (Animation)

![Demo](https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExd2VjZ3l0Z3RjZ2F5d2N4b2R0cWw1b2x6Z2Y3d3RrY3l6aG9mZ3JzZCZlcD12MV9naWZzX3NlYXJjaCZjdD1n/3o7btPCcdNniyf0ArS/giphy.gif)

---

## 📊 Dataset Overview

- 📁 Total Records: 2512  
- 🧾 Features: 16  
- 🏦 Channels: ATM, Branch, Online  
- 👥 Accounts: 495+  

---

## 🔍 Key Insights

### 💳 Transaction Analysis
- Debit Transactions: 77%  
- Credit Transactions: 23%  

👉 Users spend significantly more than they earn.

---

### 💰 Financial Flow
- Total Credit: ₹1.74 Lakhs  
- Total Debit: ₹5.73 Lakhs  

⚠️ Indicates high expense behavior.

---

### 🏦 Channel Distribution
- Branch: 868  
- ATM: 833  
- Online: 811  

✔ Balanced banking usage across channels

---

### 📉 Account Balance Insights
- Average Balance: ₹5114  
- Minimum Balance: ₹101  

⚠️ Some users fall under low-balance risk category.

---

## 🛠️ Tech Stack

- Python 🐍  
- Pandas  
- Matplotlib / Seaborn  
- LangChain  
- Groq API (LLM)  

---

## 🤖 GenAI Integration

This project uses **Groq LLM** to generate financial insights.

```python
from langchain_groq import ChatGroq
import os

os.environ["Groq_API_Key"] = "your_api_key"

groq_chat = ChatGroq(
    model="llama-3.3-70b-versatile",
    temperature=0
)

response = groq_chat.invoke("Explain spending pattern insights.")
print(response.content)
