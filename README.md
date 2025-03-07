## AI Coding Agent

## Overview
The **AI Coding Agent is a AI assistant that helps users solve coding problems by leveraging **OpenAI GPT-4o, Google Gemini, and an execution sandbox**. It allows users to:

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

### **3️⃣ Set Up API Keys**
Create a `.env` file or enter keys in the Streamlit sidebar:
- **OpenAI API Key** (for GPT-4o)
- **Google Gemini API Key** (for image processing)
- **E2B API Key** (for sandbox execution)

### **4️⃣ Run the Streamlit App**
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

## License
📜 This project is licensed under the **MIT License**.

# 💻 Multimodal AI Coding Agent Team with o3-mini and Gemini
An AI Powered Streamlit application that serves as your personal coding assistant, powered by multiple Agents built on the new o3-mini model. You can also upload an image of a coding problem or describe it in text, and the AI agent will analyze, generate an optimal solution, and execute it in a sandbox environment.

## Features
#### Multi-Modal Problem Input
- Upload images of coding problems (supports PNG, JPG, JPEG)
- Type problems in natural language
- Automatic problem extraction from images
- Interactive problem processing

#### Intelligent Code Generation
- Optimal solution generation with best time/space complexity
- Clean, documented Python code output
- Type hints and proper documentation
- Edge case handling

#### Secure Code Execution
- Sandboxed code execution environment
- Real-time execution results
- Error handling and explanations
- 30-second execution timeout protection

#### Multi-Agent Architecture
- Vision Agent (Gemini-2.0-flash) for image processing
- Coding Agent (OpenAI- o3-mini) for solution generation
- Execution Agent (OpenAI) for code running and result analysis
- E2B Sandbox for secure code execution

## How to Run

Follow the steps below to set up and run the application:
- Get an OpenAI API key from: https://platform.openai.com/
- Get a Google (Gemini) API key from: https://makersuite.google.com/app/apikey
- Get an E2B API key from: https://e2b.dev/docs/getting-started/api-key

1. **Clone the Repository**
   ```bash
   git clone https://github.com/Shubhamsaboo/awesome-llm-apps.git
   cd ai_agent_tutorials/ai_coding_agent_o3-mini
   ```

2. **Install the dependencies**
    ```bash
    pip install -r requirements.txt
    ```

3. **Run the Streamlit app**
    ```bash
    streamlit run ai_coding_agent_o3.py
    ```

4. **Configure API Keys**
   - Enter your API keys in the sidebar
   - All three keys (OpenAI, Gemini, E2B) are required for full functionality

## Usage
1. Upload an image of a coding problem OR type your problem description
2. Click "Generate & Execute Solution"
3. View the generated solution with full documentation
4. See execution results and any generated files
5. Review any error messages or execution timeouts
# AI-Coding-Agent-
