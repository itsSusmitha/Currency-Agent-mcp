# Currency-Agent-mcp
LLM based currency conversion agent using tools
# 💱 Currency Conversion Agent using LLM Tools (MCP Style)

## 📌 Overview
This project demonstrates a **tool-augmented AI agent** built using an LLM (Gemini) that performs currency conversion using multiple custom tools.

The agent follows a **Model Context Protocol (MCP)-style workflow**, where different tools handle different parts of the task such as fee lookup, exchange rate retrieval, and final calculation using a code executor.

---

## ⚙️ Features
- 💳 Retrieves transaction fee based on payment method  
- 💱 Fetches real-time (simulated) currency exchange rates  
- 🧮 Performs final currency conversion with fee deduction  
- 🤖 Uses LLM agent to decide which tools to use  
- 🧑‍💻 Executes Python code using a built-in code executor  
- 🔁 Handles errors using structured tool responses  

---

## 🧠 Architecture / Workflow

User Request  
⬇️  
LLM Agent (Gemini)  
⬇️  
1. Fee Tool → gets transaction fee %  
2. Exchange Rate Tool → gets currency rate  
3. Calculation Agent → generates Python code  
4. Code Executor → runs code  
⬇️  
Final Output (Converted Amount)

---

## 🛠️ Tools Used

### 1. Fee Lookup Tool
Returns transaction fee based on payment method:
- Credit Card → 2%
- Debit Card → 3.5%
- Bank Transfer → 1%

### 2. Exchange Rate Tool
Returns currency conversion rates between:
- USD → INR / EUR / JPY

### 3. Calculation Agent
- Generates Python code for computation  
- Ensures correct calculation of:
  - Converted amount  
  - Fee deduction  
  - Final payout  

---

## 💡 Example

### Input:
Convert 100 USD to INR using platinum credit card

### Process:
- Exchange rate fetched (USD → INR)
- Fee applied (2%)
- Calculation executed via Python code

### Output:
Final amount after fee deduction and conversion

---

## 🚀 Tech Stack
- Python  
- Gemini LLM (LLM Agent)  
- Tool-based architecture (MCP-style)  
- Built-in Code Executor  

---

## 📚 Key Learnings
- How LLM agents use external tools  
- Multi-tool orchestration (agent workflows)  
- MCP-style modular AI design  
- Code generation + execution pipelines  
- Real-world AI system architecture  

---

## 📌 Future Improvements
- Connect to real exchange rate API  
- Add more payment methods  
- Build UI for user interaction  
- Deploy as web app  

---

## 👨‍💻 Author
Built as part of an AI Agent + MCP learning project.

---
