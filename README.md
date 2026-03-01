# grading_powerbi_projects_with_openai

## Overview

This repository contains a **Python Jupyter Notebook** designed to automate the evaluation of student data analysis assignments. The notebook processes **PDF submissions** that include dashboards, visuals, and summary reports, then generates structured, rubric-based grades and feedback.  

The system is intended to assist instructors in grading **multi-perspective business analysis assignments** using the **AdventureWorks dataset** (a simulated bicycle manufacturing and sales company dataset).

---

## Features

- **PDF Processing**
  - Reads student submissions containing dashboards, charts, KPIs, and textual summaries.
  - Extracts relevant visual and textual content for evaluation.
  
- **Automated Grading**
  - Applies a **multi-criteria rubric**, evaluating:
    - Relevance of perspective
    - Correctness of analysis and joins
    - Visualization clarity
    - Insights and recommendations
    - Methodology and assumptions
    - Presentation and formatting
  - Generates **justified scores** for each criterion.

- **Structured Output**
  - Produces **JSON files** for each student containing:
    - Individual rubric scores
    - Total score
    - Strengths and areas for improvement
  - Supports integration into grading dashboards or analytics pipelines.

- **Batch Processing**
  - Handles multiple student submissions in a single run.
  - Supports organizing PDFs by student ID.

---

## How It Works

1. **Input**
   - Excel or CSV file with student submission links (Google Drive or local paths) and student identifiers.
   - PDFs submitted by students (Power BI dashboards + written summary).

2. **Processing**
   - Extracts key content from PDFs (tables, charts, KPIs, textual summaries).
   - Performs rubric-based evaluation using a grading logic layer (prompt-based or rule-based).

3. **Output**
   - JSON file per student containing:
     - Scores per rubric category
     - Total score
     - Feedback (strengths and improvement areas)

---
#NOTE
Rubric and AI model may need to be tweaked to improve performance.
