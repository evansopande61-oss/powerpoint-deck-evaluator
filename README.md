# Evans Opande - PowerPoint Deck Evaluator

[![Python](https://img.shields.io/badge/Python-3.11-blue)]()
[![AI](https://img.shields.io/badge/AI-Deck%20Evaluation-purple)]()
[![NLP](https://img.shields.io/badge/NLP-Content%20Analysis-yellow)]()
[![License](https://img.shields.io/badge/License-MIT-green)]()

An AI-powered PowerPoint deck evaluation system that analyzes presentation slides for content quality, visual design, structure, readability, and overall presentation effectiveness.

---

## Project Overview

This project evaluates PowerPoint presentations and generates professional feedback reports.

The system reviews slide decks based on:

- Content clarity
- Slide structure
- Visual design
- Readability
- Storytelling flow
- Grammar and wording
- Audience alignment
- Presentation impact

---

## Features

### PowerPoint Analysis

- Upload `.pptx` files
- Extract slide text
- Analyze slide layout
- Detect slide count and structure
- Identify missing titles or weak sections

### Content Evaluation

- Clarity scoring
- Grammar review
- Message quality analysis
- Slide-by-slide feedback
- Executive summary generation

### Design Evaluation

- Font consistency checking
- Color consistency analysis
- Visual balance scoring
- Text density detection
- Readability assessment

### Report Generation

- Overall deck score
- Slide-by-slide recommendations
- Strengths and weaknesses
- Improvement checklist
- Exportable evaluation report

---

## Tech Stack

- Python
- python-pptx
- OpenAI / LLM APIs
- Hugging Face Transformers
- FastAPI
- Streamlit
- Pandas
- Matplotlib
- Plotly

---

## Project Structure

```text
evansopande61-oss-powerpoint-deck-evaluator/
│
├── data/
│   ├── raw/
│   └── processed/
│
├── uploads/
│
├── reports/
│
├── src/
│   ├── extract_slides.py
│   ├── content_analysis.py
│   ├── design_analysis.py
│   ├── readability_score.py
│   ├── deck_scoring.py
│   ├── report_generator.py
│   └── evaluator.py
│
├── app/
│   ├── dashboard.py
│   └── api.py
│
├── tests/
│
├── requirements.txt
├── README.md
└── LICENSE
```

---

## Installation

### Clone Repository

```bash
git clone https://github.com/evansopande61-oss/evansopande61-oss-powerpoint-deck-evaluator.git

cd evansopande61-oss-powerpoint-deck-evaluator
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

---

## Usage

### Evaluate a Deck

```bash
python src/evaluator.py --file uploads/sample_deck.pptx
```

### Launch Dashboard

```bash
streamlit run app/dashboard.py
```

### Run API Server

```bash
uvicorn app.api:app --reload
```

---

## Example Output

```json
{
  "overall_score": 87,
  "content_score": 90,
  "design_score": 84,
  "readability_score": 88,
  "structure_score": 86,
  "recommendations": [
    "Reduce text density on slides 4 and 7",
    "Add stronger section transitions",
    "Improve visual consistency across charts"
  ]
}
```

---

## Evaluation Categories

| Category | Description |
|----------|-------------|
| Content Quality | Checks clarity, relevance, grammar, and completeness |
| Visual Design | Reviews layout, spacing, color, and typography |
| Structure | Evaluates logical flow and storytelling |
| Readability | Measures text density and ease of understanding |
| Engagement | Assesses presentation impact and audience appeal |

---

## Future Improvements

- PDF Deck Support
- AI Slide Rewrite Suggestions
- Visual Layout Detection
- Brand Guideline Checking
- Investor Pitch Deck Scoring
- Academic Presentation Review
- Export to PDF Report
- Team Collaboration Dashboard
- Speaker Notes Evaluation

---

## Author

### Evans Opande

AI Engineer | Machine Learning Practitioner | Presentation AI Enthusiast

GitHub: https://github.com/evansopande61-oss

---

Built and maintained by Evans Opande — specializing in Artificial Intelligence, Machine Learning, NLP, Computer Vision, LLMs, and AI-powered productivity tools.

If you found this project useful, consider giving it a ⭐.
