# -Resume-Screening-Automation-
Objective: Automate resume filtering to match candidates with job openings.  Task Deliverables:  Extract skills and experience using spaCy or NLTK. Match resumes to job descriptions with TF-IDF or BERT. Outcome: Faster, more accurate intern selection. 📊 Data Source: Intern resume database.
# AI-Powered Resume Screener & Skill Matcher

## Project Overview
This project was developed as a specialized internship task for **Internee.pk**. It provides an automated solution for HR departments to screen resumes against specific job descriptions. The tool extracts text from PDF resumes, identifies key technical skills using Natural Language Processing (NLP), and calculates a percentage match score using machine learning techniques.

## Key Features
* **PDF Text Extraction:** Uses `PyMuPDF` (fitz) to parse and extract text from uploaded PDF documents.
* **Skill Entity Recognition:** Implements a custom `spaCy` PhraseMatcher to identify specific technical skills from a predefined database.
* **Semantic Similarity:** Utilizes `TF-IDF Vectorization` and `Cosine Similarity` via `scikit-learn` to calculate how closely a resume aligns with a job description.
* **Automated Screening:** Provides an instant match percentage, helping recruiters prioritize top candidates efficiently.

## Tech Stack
* **Python 3.x**
* **spaCy:** Industrial-strength NLP for skill extraction.
* **scikit-learn:** For TF-IDF vectorization and similarity mathematics.
* **PyMuPDF (fitz):** For high-performance PDF processing.
* **Google Colab:** Optimized for cloud-based execution and file handling.

## Mathematical Approach
The match score is calculated using **Cosine Similarity**, which measures the cosine of the angle between two vectors (the Resume and the Job Description) in a multi-dimensional space:

$$\text{Similarity} = \frac{A \cdot B}{\|A\| \|B\|}$$

This ensures that the score is based on the frequency and relevance of keywords rather than just the length of the document.
