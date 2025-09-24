# 🌍 Multi-Agent AI System for Climate Change Impact Analysis (Groq LLM)

![Python](https://img.shields.io/badge/Python-3.10+-blue)
![LangGraph](https://img.shields.io/badge/LangGraph-enabled-green)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

This project demonstrates a **multi-agent AI system** using **Groq LLM** and **LangGraph** to generate structured reports on climate change’s impact on global agriculture.  

Unlike simple retrieval tools, this system uses multiple AI agents that **plan, research, generate, reflect, and critique**, producing coherent and accurate reports.

---

## 🚀 Features

- Uses **Groq LLM** for natural language generation.  
- Implements **5 specialized agents** for a controlled, multi-step workflow:
  1. **Plan** – Defines the scope and objectives of the report.  
  2. **Research Plan** – Generates search queries to gather relevant data.  
  3. **Generate** – Drafts the report and integrates feedback.  
  4. **Reflect** – Suggests improvements for clarity, coherence, and completeness.  
  5. **Research Critique** – Provides additional queries and insights to improve the report.  
- Supports multiple **revision loops** for iterative improvements.  
- Modular and extendable to other topics or LLMs.

---

## 🛠 Workflow

1. **Plan agent** sets goals and key questions for the report.  
2. **Research Plan agent** generates up to 3 search queries for data collection.  
3. **Generate agent** produces the initial report draft using Groq LLM.  
4. If revisions are enabled, **Reflect** and **Research Critique agents** provide feedback and additional insights.  
5. **Generate agent** updates the report based on feedback.  
6. The workflow iterates until the maximum number of revisions is reached. The final report is output.

---

## 📋 Requirements

- **Groq LLM API key** – Provide via `main.py`, `.env` file, or environment variable `GROQ_API_KEY`.  
- **Optional search API** – For real-time data retrieval.  
- Python >= 3.10  
- LangGraph and LangChain libraries  

---

## 📝 Example Report

**Title:** *Climate Change Impact on Global Agriculture*

**Highlights:**

- Rising global temperatures and extreme weather events reduce crop yields.  
- Drought-prone regions in Africa and Asia face severe agricultural challenges.  
- Northern Europe benefits from longer growing seasons; Southern Europe faces water scarcity.  
- Livestock, fisheries, and crop sectors are all impacted.  
- Adaptation strategies include drought-resistant crops, improved irrigation, and early warning systems.  
- Global crop yields may decline by 10–20% by 2050 without intervention.

**Conclusion:**  
Multi-faceted approaches combining technology, policy, and local knowledge are essential to sustain agricultural productivity and ensure food security.

---

## ⚡ How to Run

1. Clone the repository:

```bash
git clone <repo_url>
cd multi-agent-climate-report
````

2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Add your **Groq API key**:

* In `.env` file:

```text
GROQ_API_KEY=your_api_key_here
```

* Or as environment variable:

```bash
export GROQ_API_KEY=your_api_key_here
```

4. Run the main script:

```bash
python main.py
```

5. View the final report output in the console or saved file.

---

## 📚 References

* Food and Agriculture Organization (FAO)
* Intergovernmental Panel on Climate Change (IPCC)
* World Bank reports and peer-reviewed research

---

## ⚖️ License

MIT License – Open for modification and research purposes.


