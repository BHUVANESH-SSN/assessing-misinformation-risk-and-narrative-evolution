# Assessing Misinformation Risk and Narrative Evolution

## Overview
Misinformation doesn't spread as single false posts. It evolves over time, changing its wording and tone across different platforms. Traditional fact-checking that just labels things "true" or "false" misses how these narratives actually develop and spread.

This project builds an AI system that analyzes misinformation at the narrative level, tracks how misleading content changes, and assigns risk scores with clear explanations.

## The Problem
Current misinformation detection systems only look at individual posts and give binary outputs. They can't:
- Track how narratives change over time
- Identify which narratives are becoming more dangerous
- Explain why something is risky

This makes it hard for journalists and fact-checkers to prioritize what needs attention.

## Our Solution
The system:
- Collects text from multiple platforms
- Converts text into numerical representations using NLP
- Groups similar misleading content to find evolving narratives
- Tracks changes in tone and framing over time
- Assigns continuous risk scores instead of true/false labels
- Provides clear explanations for why content is risky

## Key Features
- Analyzes narratives, not just individual posts
- Tracks misinformation evolution over time
- Risk-based scoring for prioritization
- Explainable AI with keywords and trends
- Scalable for real platforms

## Tech Stack
**AI/ML:** Python, PyTorch, Hugging Face, Sentence Transformers, BERTopic, FAISS, Scikit-learn

**NLP/Explainability:** KeyBERT, Captum, spaCy, NLTK

**Backend/UI:** FastAPI, Streamlit, Plotly

## Installation
```bash
git clone https://github.com/BHUVANESH-SSN/assessing-misinformation-risk-and-narrative-evolution.git
cd assessing-misinformation-risk-and-narrative-evolution
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

## Running the App

Streamlit UI:
```bash
streamlit run frontend/app.py
```

FastAPI Backend:
```bash
uvicorn app.main:app --reload
```

## What You Get
- Narrative clusters showing evolving misinformation
- Risk scores indicating harm level
- Explainable insights with keywords and emotional triggers
- Interactive visualizations

## Impact
- Early detection of harmful narratives
- Helps prioritize critical content
- Transparent and explainable results
- Reduces manual work by grouping related content

## Future Plans
- Real-time social media monitoring
- Multilingual support
- Network propagation modeling
- Integration with fact-checking APIs

## Author
Bhuvanesh S  
B.E. Computer Science and Engineering