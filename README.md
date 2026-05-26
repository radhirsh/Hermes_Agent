# 📑🤖 Hermes Agent – Enterprise Contract Intelligence System

An Agentic AI Contract Intelligence System using Hermes Agent to read contracts, detect risks, evaluate confidence, and decide when legal review is actually needed.

Built for enterprise contract analysis using intelligent task planning, tool orchestration, clause extraction, and risk-based legal escalation.

---

## 🚀 Overview

Contract reviews in enterprises are often manual, time-consuming, and error-prone.

Legal and procurement teams spend hours reviewing:

- Vendor Agreements
- NDAs
- Master Service Agreements (MSA)
- Statements of Work (SOW)

to identify:

❌ Missing clauses  
❌ Legal risks  
❌ Compliance gaps  
❌ Weak liability definitions  
❌ Undefined SLAs  
❌ Missing termination conditions

This project uses **Hermes Agent** to automate enterprise contract understanding through **agentic reasoning, task planning, and intelligent tool orchestration**.

Instead of simply summarizing contracts, Hermes decides:

> What to analyze, what risks matter, and when escalation is actually needed.

---

## ✨ Features

### 📄 Contract Understanding
- NDA Analysis
- Vendor Agreement Review
- MSA Evaluation
- SOW Intelligence

### 🧠 Agentic Planning
Hermes dynamically plans:

```text
Read Contract
      ↓
Identify Contract Type
      ↓
Extract Clauses
      ↓
Detect Risks
      ↓
Check Compliance
      ↓
Calculate Confidence
      ↓
Recommend Action
```

### ⚠️ Risk Detection
Detects:

- Missing termination clauses
- Weak liability definitions
- Undefined SLAs
- Compliance issues
- Business risks
- Missing confidentiality sections

### 🛠 Tool Orchestration
Hermes invokes multiple tools dynamically:

- PDF Parsing
- Clause Extraction
- Risk Analysis
- Compliance Validation
- Summary Generation

### 📈 Confidence-Based Decisioning
Instead of escalating every contract:

Hermes calculates:

```text
Risk Score
+
Confidence Score
```

to determine:

```text
Approve
or
Escalate to Legal Review
```

---

# 🏗 Architecture

```text
                Contract PDF
                       │
                       ▼
            Hermes Master Agent
                       │
             Task Planning Layer
                       │
      ┌────────────────────────────────┐
      │                                │
      ▼                                ▼
 PDF Parsing Tool              Contract Type Detection
      │                                │
      └──────────────┬─────────────────┘
                     ▼
              Clause Extraction
                     │
                     ▼
               Risk Detection
                     │
                     ▼
            Compliance Validation
                     │
                     ▼
             Confidence Scoring
                     │
                     ▼
            Executive Summary
                     │
                     ▼
          Legal Review Recommendation
```

---

## 🧩 Example Workflow

### Input

Upload:

```text
vendor_agreement.pdf
```

### Hermes Agent Plan

```text
1. Read uploaded contract
2. Identify contract type
3. Extract important clauses
4. Detect missing sections
5. Evaluate business risk
6. Calculate confidence
7. Decide escalation
```

### Output

```text
Contract Type:
Vendor Agreement

Risk Score:
7.8/10

Detected Issues:
❌ Missing termination clause
❌ SLA definition unclear
⚠ Weak liability section

Confidence:
89%

Recommendation:
Escalate to Legal Review
```

Low-risk contract example:

```text
Contract Type:
NDA

Risk Score:
2.3/10

Detected Issues:
✅ Confidentiality clause present
✅ Termination clause present

Confidence:
95%

Recommendation:
Approved
```

---

## ⚙️ Tech Stack

### Core Framework
- Hermes Agent

### Backend
- FastAPI
- Python

### LLM & AI
- Azure OpenAI
- LangChain

### Document Processing
- PDFPlumber
- PyPDF

### Frontend
- Streamlit

### Data Processing
- Pydantic

---

## 📂 Project Structure

```text
hermes_agent/

│── app/
│   ├── agents/
│   │   ├── master_agent.py
│   │   ├── risk_agent.py
│   │   └── compliance_agent.py
│   │
│   ├── tools/
│   │   ├── pdf_parser.py
│   │   ├── clause_extractor.py
│   │   ├── risk_detector.py
│   │   └── summary_generator.py
│   │
│   ├── api/
│   │   └── routes.py
│   │
│   ├── schemas/
│   │   └── contract_schema.py
│   │
│   └── services/
│       └── llm_service.py
│
│── uploads/
│
│── main.py
│── requirements.txt
│── README.md
```

---

## 🔧 Installation

Clone repository

```bash
git clone https://github.com/radhirsh/hermes_agent.git
```

Move into project

```bash
cd hermes_agent
```

Install dependencies

```bash
pip install -r requirements.txt
```

Run application

```bash
uvicorn main:app --reload
```

FastAPI docs:

```text
http://127.0.0.1:8000/docs
```

---

## 🧪 API Example

### Upload Contract

```http
POST /analyze_contract
```

Request:

```json
{
  "contract_text":
  "Vendor agreement content"
}
```

Response:

```json
{
  "contract_type":
  "Vendor Agreement",

  "risk_score":
  0.83,

  "confidence":
  0.91,

  "recommendation":
  "Legal Review"
}
```

---

## 🧠 How Hermes Agent Powers This Project

Hermes Agent acts as the **orchestration brain** of the system.

Instead of using hardcoded workflows, Hermes:

### 1. Plans Tasks

Hermes determines:

```text
What to do next
```

based on contract content.

---

### 2. Uses Tools Dynamically

Hermes invokes:

```python
parse_pdf()

extract_clauses()

risk_detector()

compliance_checker()

summary_generator()
```

depending on contract type and context.

---

### 3. Multi-Step Reasoning

Hermes reasons through:

```text
Contract Type
↓
Risk Signals
↓
Missing Clauses
↓
Confidence Level
↓
Escalation Decision
```

This makes the system behave closer to a **real enterprise legal analyst**.

---

## 📸 Screenshots

### Upload Interface

_Add screenshot here_

### Hermes Planning Workflow

_Add screenshot here_

### Contract Analysis Output

_Add screenshot here_

---

## 🎥 Demo Video

_Add video/GIF here_

---

## 🔮 Future Improvements

- Multi-language contracts
- OCR support
- Contract comparison
- Clause benchmarking
- Compliance knowledge graph
- Human-in-the-loop approvals
- Risk explainability dashboard

---

## 🤝 Contributing

Contributions are welcome.

Feel free to fork, improve, and create pull requests.

---

## 👨‍💻 Author

### Sridhar S

AI/ML Engineer | Generative AI | Agentic AI | RAG Systems

🔗 LinkedIn  
http://linkedin.com/in/sridhar-s-076337178

💻 GitHub  
http://github.com/radhirsh

---

## ⭐ Support

If you found this useful, consider giving the repository a **star** ⭐

It helps and motivates future improvements 🚀
