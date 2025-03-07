## AI Coding Agent

## Overview
The AI Coding Agent is a AI assistant that helps users solve coding problems by leveraging **OpenAI GPT-4o, Google Gemini, and an execution sandbox**. It allows users to:

✅ **Upload coding problems as text or images**

✅ **Generate Python solutions using AI**

✅ **Execute generated code in a secure sandbox**

✅ **Receive detailed execution logs and error explanations**

---

## Features
### 🔹 AI-Powered Code Generation
- Uses **GPT-4o** to generate **optimized Python solutions**.
- Supports **automated error handling and best coding practices**.

### 🔹 Image Processing with Gemini
- Upload an image of a coding problem.
- The **Gemini Vision model** extracts and interprets the problem statement.

### 🔹 Secure Code Execution
- Runs AI-generated code in an **E2B sandbox**.
- Supports **error handling, execution time limits, and security isolation**.

### 🔹 User-Friendly Streamlit UI
- **Interactive interface** with API key input fields.
- Options to **input coding problems as text or images**.
- **Live execution feedback** with logs and results.

---

## Installation & Setup

### Get API Keys
- Get an OpenAI API key from: https://platform.openai.com/
- Get a Google (Gemini) API key from: https://makersuite.google.com/app/apikey
- Get an E2B API key from: https://e2b.dev/docs/getting-started/api-key

### **1️⃣ Clone the Repository**
```bash
git clone https://github.com/eddiepiper/AI-Coding-Agent-.git
cd ai-coding-agent
```

### **2️⃣ Install Dependencies**
```bash
pip install -r requirements.txt
```

### **3️⃣ Run the Streamlit App**
```bash
streamlit run ai_coding_agent_o3.py
```

---

## Usage Guide
1️⃣ **Enter API keys** in the Streamlit sidebar.

2️⃣ **Input a coding problem** (text OR image).

3️⃣ **Click 'Generate & Execute Solution'**.

4️⃣ **View AI-generated code** and execution results.

---

## Example
### **Input (Text-Based Problem)**
```python
"Write a function to calculate Fibonacci numbers."
```

### **Output (AI-Generated Solution)**
```python
def fibonacci(n: int) -> int:
    if n <= 0:
        return 0
    elif n == 1:
        return 1
    return fibonacci(n-1) + fibonacci(n-2)
```

### **Execution Result**
```
✅ Function executed successfully
✅ Sample input: fibonacci(5) → Output: 5
```

---

## Troubleshooting

**Error: `No event loop in thread 'ScriptRunner'`**

🔹 **Solution:** Add `import nest_asyncio` and `nest_asyncio.apply()` at the beginning of the script.

**Error: `google-genai not installed`**

🔹 **Solution:** Run `pip install google-genai`.

---

## Contributing
🚀 We welcome contributions! Feel free to fork this repo, submit issues, or create pull requests.

---
