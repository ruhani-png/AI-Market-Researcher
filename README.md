# 📘 Market Research Assistant  
### Machine Learning for Business – Individual Coursework  

This project implements a Market Research Assistant that uses Large Language Models (LLMs) and Wikipedia retrieval to generate industry-specific reports. It was developed as part of the Machine Learning for Business module at UCL.

---

## 📦 Requirements

Before running the notebook, install the required libraries:

```bash
pip install langchain-google-genai
pip install langchain-community
pip install wikipedia
```

## ⚙️ Setup
The environment setup includes:
- Importing libraries for data handling, web requests, and LLM interactions
- Setting Wikipedia language to English
- Patching BeautifulSoup integration for Wikipedia retrieval

## 🧠 Model Workflow
### 1. Information Retrieval
  - Wikipedia is queried using `WikipediaRetriever` from `LangChain`.
  - Text content is preprocessed and formatted for the LLM.
### 2. LLM Prompting
  - A system prompt is defined to guide the LLM's behaviour for report generation.
  - `ChatGoogleGenerativeAI` or OpenAI's GPT is used depending on setup.
### 3. Report Generation
  - Based on user queries, the assistant generates structured responses.
  - Each report includes analysis on market size, trends, competitors, and strategic recommendations.
### 4. Evaluation
  - Reports are scored on quality and relevance using evaluation metrics defined in the notebook.

## 📊 Outputs
- Detailed industry-specific reports for multiple questions 
- Evaluation metrics printed alongside the generated content

## 🧪 Testing
You can run the report generation by executing the final section of the notebook, which loops over a list of predefined questions and industries.

## 📁 File Structure
- `ML_Individual_CW_Final (2).ipynb`: Main notebook with all code and logic.
- Uses external APIs (Wikipedia, LLMs) and requires internet access.

