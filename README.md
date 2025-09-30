🌟 CryptoWise: Your First AI-Powered Financial Sidekick! 🌟
Overview
CryptoWise is a rule-based cryptocurrency advisor chatbot created as the Week 1 assignment for the PLP Academy. Its core function is to provide basic investment advice by analyzing pre-defined data based on two crucial factors: profitability (price trends and market cap) and sustainability (energy efficiency and eco-score).

This project demonstrates the basics of AI-driven decision-making using simple Python logic.

💡 How It Mimics AI Decision-Making
The chatbot operates on a simple but effective if-else logic model:

Input Processing: It listens for keywords in your query (e.g., "sustainable," "profit," "long-term").

Rule Application: It matches the query to one of three hardcoded Advice Rules (Profitability, Sustainability, or General Growth).

Data Lookup: It retrieves the corresponding best recommendation from the crypto_db based on the rule's criteria (e.g., finding the coin with the highest sustainability_score).

Output: It provides a deterministic, data-backed answer.

⚙️ Setup and Execution
Prerequisites
Python 3.x

A Python IDE (like VS Code) or a Jupyter Notebook environment (like Google Colab or Jupyter Notebook).

Running the Chatbot
Clone this repository or copy the code from chatbot.py (or the .ipynb file).

Open your Python environment (e.g., a Jupyter Notebook cell).

Execute the run_chatbot() function.

The bot will launch and prompt you for input in the terminal/output window.

Python

# To start the chatbot
run_chatbot()
🤖 Sample Conversation
You can ask CryptoWise about three main investment goals:

Goal	Sample Query	CryptoWise Response (Example)
Profitability	Which coin is trending up for a quick profit?	For short-term profitability, Bitcoin is the top pick. It has the best combination of momentum and market depth. 📈
Sustainability	What's the most eco-friendly coin to invest in?	Invest in Cardano! 🌱 It has the highest sustainability score (8/10) and low energy use...
Long-Term Growth	Which crypto should I buy for long-term growth?	For long-term growth and stability, consider Cardano. It's currently trending up (🚀) and is highly sustainable...

Export to Sheets
📊 Predefined Crypto Data
The chatbot's advice is based on this internal, static dataset:

Python

crypto_db = {  
    "Bitcoin": {  
        "price_trend": "rising",  
        "market_cap": "high",  
        "energy_use": "high",  
        "sustainability_score": 3/10  
    },  
    "Ethereum": {  
        "price_trend": "stable",  
        "market_cap": "high",  
        "energy_use": "medium",  
        "sustainability_score": 6/10  
    },  
    "Cardano": {  
        "price_trend": "rising",  
        "market_cap": "medium",  
        "energy_use": "low",  
        "sustainability_score": 8/10  
    }
}
🛑 Important Disclaimer
⚠️ Disclaimer: This project is for educational purposes only and uses static, simplified data. Cryptocurrency investment is highly volatile and risky. This is not financial advice. Always do your own research before investing.
