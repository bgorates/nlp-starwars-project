# Galactic Identification System 🌌

**A Natural Language Processing (NLP) Project to Identify Star Wars Characters from Dialogue.**

## 📌 Project Overview
This project focuses on predicting the identity of Star Wars characters based solely on their dialogue lines from the Original Trilogy (Episodes IV, V, VI).

The system uses **Classical Machine Learning (Logistic Regression)** and **TF-IDF Vectorization** to classify text into character classes. It handles data ingestion, preprocessing (stemming, stopword removal), and complex benchmarking using confusion matrices.

## 📂 Repository Contents
* `Galactic_Identification_System.ipynb`: The main Jupyter Notebook containing all code, visualizations, and the demo application.
* `prompt_log.txt`: A log of AI prompts used to assist in code generation (Required for course compliance).

## 🚀 How to Run the Project
The easiest way to view and run the code is via **Google Colab**:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1QN1Mk3uFC2jcREJfydEnLTQGUW71qdVG?usp=sharing)

1.  Click the "Open in Colab" badge above.
2.  In Colab, go to **Runtime > Run All** to execute the pipeline.
3.  Scroll to the bottom to try the **Interactive Demo** where you can type your own quotes!

## 🛠️ The Pipeline
The project follows a standard Data Science lifecycle:

1.  **Data Ingestion:** Parsed raw text scripts from GitHub using `requests` (handling inconsistent formatting).
2.  **Preprocessing:**
    * Lowercase & Special Character removal.
    * **Stopword Removal** (NLTK).
    * **Stemming** (PorterStemmer) to normalize words (e.g., "escaping" -> "escap").
    * *Verified via Unit Tests.*
3.  **Visualization (EDA):**
    * Bar Charts for character line counts.
    * Word Clouds to visualize distinct vocabularies (e.g., Yoda vs. Han Solo).
4.  **Model Training:**
    * **Vectorization:** TF-IDF (Term Frequency-Inverse Document Frequency).
    * **Classifier:** Logistic Regression.
5.  **Evaluation:**
    * Accuracy Score.
    * Confusion Matrix (Visualizing misclassifications).

## 📊 Results
* **Overall Accuracy:** ~38% (vs. 10% random chance baseline).
* **Key Findings:**
    * **Red Leader:** 100% Precision (Due to distinct military jargon).
    * **Han Solo / Luke:** High confusion rate (Shared screen time and casual dialect).
    * **Yoda:** Lower detection rate due to class imbalance (fewer lines of dialogue).

## 🤖 AI Usage Disclosure
In accordance with course requirements, this project utilized a Generative Language Model to assist with syntax generation and debugging.
* **Tool:** Google Gemini / Colab AI.
* **Prompt Log:** See `prompt_log.txt` for the full record of prompts used.

## 👤 Author
* **Neptun Code:** M3N8YE
