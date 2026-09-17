# Student Feedback Sentiment Analysis

## 📌 Project Overview

This project analyzes student feedback using Natural Language Processing (NLP) techniques and classifies feedback into:

- Positive
- Negative
- Neutral

The system supports student feedback from CSV/Excel files and also includes voice-to-text processing for audio feedback.

## 🎯 Objectives

- Automatically analyze student feedback
- Clean and preprocess textual feedback
- Classify feedback based on sentiment
- Combine feedback from multiple questions
- Generate sentiment results for analysis and visualization
- Support text and voice-based feedback

## 🛠️ Technologies Used

- Python
- Pandas
- NLTK
- VADER Sentiment Analysis
- TextBlob
- Matplotlib
- Plotly
- SpeechRecognition
- PyDub
- Unidecode
- OpenPyXL

## 🔄 Project Workflow

Student Feedback  
↓  
CSV / Excel / Voice Input  
↓  
Text Preprocessing  
↓  
Text Cleaning & Normalization  
↓  
Sentiment Analysis  
↓  
VADER + TextBlob  
↓  
Rule-based Classification  
↓  
Positive / Negative / Neutral  
↓  
Results & Visualization

## 🧹 Text Preprocessing

The project performs preprocessing of student feedback before sentiment classification.

The process includes:

- Text cleaning
- Newline and whitespace normalization
- Text normalization
- Lowercase conversion where required
- Combining multiple feedback fields
- Handling empty or invalid text

## 🧠 Sentiment Analysis

### VADER

VADER (Valence Aware Dictionary and sEntiment Reasoner) is used as the primary rule-based sentiment analyzer.

The compound score is used for classification:

- Compound score ≥ 0.05 → Positive
- Compound score ≤ -0.05 → Negative
- Otherwise → Neutral

### TextBlob

TextBlob is used as a secondary sentiment analyzer when the VADER result is Neutral.

## 📂 Input

The system supports:

- CSV files
- Excel (.xlsx) files
- Text feedback
- Audio input

## 📊 Output

The system generates sentiment classifications for student feedback.

Example:

**Input:**
> The session was very helpful and I learned a lot.

**Output:**
> Positive

## 🚀 How to Run

### 1. Clone the repository

```bash
git clone https://github.com/krutika018/student-feedback-sentiment-analysis.git
