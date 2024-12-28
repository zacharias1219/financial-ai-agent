# **Building a Financial AI Agent Using PhiData**

This project demonstrates creating an end-to-end **financial analysis AI agent** using **PhiData**, an open-source framework for developing, deploying, and monitoring agentic AI systems. The project highlights practical implementation steps for constructing autonomous AI agents capable of financial analysis using multimodal models and web integration.

---

## **Features**

- **Agentic AI Development**:
  - Build independent AI agents for specific tasks like financial analysis and web searching.
  - Combine agents into a cohesive workflow for complex tasks.
  
- **Open Source and Scalable**:
  - Utilizes PhiData to enable open-source integration with various Large Language Models (LLMs).
  - Compatible with open-source libraries like Hugging Face and Groq.

- **Real-World Financial Applications**:
  - Analyze stock recommendations and generate reports using tools like `YFinance` and `DuckDuckGo`.
  - Fetch live news and market sentiments about specific stocks.

---

## **Tech Stack**

- **Framework**: PhiData
- **Backend Tools**:
  - YFinance for stock data.
  - DuckDuckGo for web search.
- **Models**: Hugging Face Transformers, Groq
- **Deployment**:
  - FastAPI for building APIs.
  - PhiData Playground for testing workflows.

---

## **Setup and Installation**

### **Prerequisites**

- **Python 3.9 or above**
- **PhiData Account**: Obtain API keys from the PhiData platform.

### **Steps**

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/yourusername/financial-ai-agent.git
   cd financial-ai-agent
   ```

2. **Create Virtual Environment**:

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install Requirements**:

   ```bash
   pip install -r requirements.txt
   ```

4. **Set Up API Keys**:
   - Create a `.env` file in the root directory.
   - Add the following keys:

     ```env
     PHIDATA_API_KEY=your_phidata_api_key
     GROQ_API_KEY=your_groq_api_key
     OPENAI_API_KEY=your_openai_api_key
     ```

5. **Run the Application**:

   ```bash
   python financial_agent.py
   ```

 6. **Output**:

    ![image](https://github.com/user-attachments/assets/007fc92c-7fb4-4ef4-828d-c5a6facc01b8)

---

## **Directory Structure**

```bash
├── agents
│   ├── financial_agent.py
│   └── web_search_agent.py
├── playground
│   └── playground.py
├── requirements.txt
└── README.md
```

---

## **Workflow Overview**

### **Independent Agents**

1. **Web Search Agent**:
   - Searches the web for relevant financial news using DuckDuckGo.
   - Integrates LLM for summarizing results.

2. **Financial Agent**:
   - Analyzes stock fundamentals, technical indicators, and recommendations using YFinance.

### **Multimodal Agent**

- Combines Web Search Agent and Financial Agent to provide detailed financial insights.

---

## **Deployment**

1. **Local Deployment**:
   - Use FastAPI to host the application locally.
   - Access endpoints via `http://localhost:8000`.

2. **PhiData Playground**:
   - Deploy agents in the PhiData platform for seamless testing and integration.

---

## **Future Enhancements**

- Extend support for additional financial tools.
- Incorporate chat-based UI for real-time agent interaction.
- Add more robust error handling and scalability features.

---

## **Contributing**

We welcome contributions! Please fork the repository, create a new branch for your feature, and submit a pull request.

---

## **License**

This project is licensed under the MIT License. See `LICENSE` for more details.

---
