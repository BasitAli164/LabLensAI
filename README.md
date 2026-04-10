<div align="center">

# 🧬 LabLensAI  
### AI-Powered Lab Report Interpreter for Patients

[![Built with Streamlit](https://img.shields.io/badge/Built%20with-Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)](https://streamlit.io)
[![AI Powered](https://img.shields.io/badge/AI--Powered-Groq%20Llama%203.3-orange?style=for-the-badge)](https://groq.com)
[![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)

**Empowering patients by translating complex medical reports into clear, actionable health insights.**

[🚀 Live Demo](https://lablensai.streamlit.app/) ·  
[📋 Technical Overview](#-technical-architecture) ·  
[⚕️ Medical Disclaimer](#-medical-disclaimer)

</div>

---

## 🌟 What Problem Does LabLensAI Solve?

Medical lab reports are written for doctors — not patients.

Patients often receive:
- Confusing numbers  
- Medical jargon  
- No clear explanation of what’s *normal*, *borderline*, or *serious*

**LabLensAI bridges this gap.**

It transforms raw lab reports into **easy-to-understand explanations**, highlights **abnormal results**, and guides users on **what to do next** — safely and responsibly.

---

## 🧪 What LabLensAI Does

- 📄 Accepts **PDF lab reports** or **pasted lab text**
- 🔍 Extracts key medical values automatically
- 🚦 Flags results as **Normal / Borderline / Abnormal**
- 🧠 Explains what each parameter means in **simple language**
- 🔗 Detects patterns across multiple tests (e.g. anemia, infection)
- 💬 Provides a **context-aware AI medical assistant**
- 🏃 Generates a **personalized health coach plan**
- 🌍 Supports **multi-language summaries**

---

## 🔄 How It Works (Simple Flow)

1. **User Uploads Report**  
   PDF or raw lab text

2. **AI Extraction**  
   LLM converts unstructured text into structured clinical data

3. **Analysis Engine**
   - Rule-based medical validation
   - Multi-parameter reasoning
   - Grounded medical explanations

4. **Dashboard**
   - Visual cards for each test
   - Risk indicators
   - AI chat + health coach

---

## 🏗️ Technical Architecture

LabLensAI uses a **hybrid GenAI + deterministic system** to stay accurate and safe.

```mermaid
graph LR
    A[User Input: PDF / Text] --> B[LLM Extraction]
    B --> C[Structured JSON]
    C --> D[Rule-Based Risk Scoring]
    C --> E[Pattern Detection]
    C --> F[Medical Knowledge Retrieval]
    D & E & F --> G[Session State]
    G --> H[Interactive Dashboard]
    H --> I[AI Medical Assistant]
    H --> J[Health Coach Plan]
```

---

## 🧠 GenAI Features (Judge-Friendly)

### 1️⃣ Structured AI Extraction
Instead of brittle regex, LabLensAI uses LLM-based extraction to handle:
- Any lab format
- Any hospital layout
- Messy or partial reports

### 2️⃣ Grounded Medical Explanations (RAG)
AI explanations are not hallucinated. Each explanation is generated using:
- Verified medical definitions
- Reference ranges
- Controlled prompts
The AI is strictly instructed to explain — never diagnose or prescribe.

### 3️⃣ Multi-Parameter Reasoning
LabLensAI doesn’t analyze values in isolation.
Examples:
- **Low Hemoglobin + Low MCV** → Possible anemia pattern
- **High WBC + Neutrophils** → Infection indicators
- **Creatinine + Urea** → Kidney health context

### 4️⃣ AI Confidence Scoring
Each analysis includes a confidence score based on:
- Extraction reliability
- Number of available parameters
- Strength of detected medical patterns

---

## 🧩 Code Structure (Simplified)

- **`app.py`** — Streamlit UI & layout
- **`extractor.py`** — LLM + regex fallback extraction
- **`analyzer.py`**
  - Risk scoring
  - Pattern detection
  - Summary & health coach generation
- **`chat_handler.py`** — Context-aware AI assistant
- **`reference_ranges.py`** — Medical ground truth

---

## 🌍 Multi-Language Support

LabLensAI supports instant translation of summaries into:
- Spanish
- Urdu
- Hindi
- Arabic
- French
- German

Healthcare clarity should be global.

---

## ⚠️ Current Limitations

- Image OCR is experimental (PDF & text work best)
- Focused on common panels (CBC, LFT, KFT, Lipids)
- One report at a time (longitudinal analysis planned)

---

## ⚕️ Medical Disclaimer

LabLensAI is an educational tool only. It does not replace professional medical advice, diagnosis, or treatment. Always consult a qualified healthcare provider for medical decisions.

---

<div align="center">

Built for the Hugging Face Medical Hackathon
🧬 LabLensAI — Your Health, Decoded.

</div>
