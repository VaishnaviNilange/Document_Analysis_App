# Document_Analysis_App
Repository Structure:
Document_Analysis_App/
│
├── main.py                # Streamlit app main file
├── text_extraction.py     # All text extraction logic
├── comparison.py          # Document comparison logic
├── requirements.txt       # All dependencies
├── README.md              # Project info and usage
├── .gitignore
└── sample_documents/      # Sample PDFs, DOCX, TXT for testing


## Overview
This Streamlit-based app allows users to upload documents (PDF, DOCX, TXT) and instantly extract insights, summarize content, perform Q&A, and compare multiple documents.

---

## Features
- **Document Upload:** Supports PDF, DOCX, and TXT files
- **Text Extraction:** Extracts clean text for analysis
- **Summarization:** AI-based summarization for long documents
- **Q&A:** Ask questions about your document content
- **Key Insights:** Automatically generates key points
- **Document Comparison:** Compare two PDFs to spot differences

---

## How It Works
1. Upload your document(s)
2. Text is extracted and analyzed using **transformers & Groq AI**
3. Results are displayed in an interactive Streamlit dashboard
4. Optionally, compare two PDFs side-by-side

---

## Installation
```bash
git clone https://github.com/<YOUR_GITHUB_USERNAME>/Document_Analysis_App.git
cd Document_Analysis_App
python -m venv .venv
.\.venv\Scripts\activate   # Windows
pip install -r requirements.txt
streamlit run main.py
