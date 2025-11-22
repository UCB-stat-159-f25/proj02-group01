[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/7TPcE591)

# Project 2: Reproducibility in Natural Language Processing

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/UCB-stat-159-f25/proj02-group01/HEAD)

## Overview

This project investigates the **reproducibility of Natural Language Processing (NLP) analyses** using the **State of the Union (SOTU) speech dataset**.

The work in this repository includes:

- **Part 1:** Data loading and exploratory data analysis (EDA)  
- **Part 2:** Text processing with SpaCy, TF-IDF vectorization, and dimensionality reduction  
- **Part 3:** Topic modeling using LDA and BERTopic  
- **Part 4:** Additional analyses, including word frequency trends over time  

All work is performed in a fully **reproducible Jupyter Notebook environment**, as specified in `environment.yml`.

You can launch the notebooks directly in your browser using **Binder** by clicking the Binder badge. Binder will automatically set up JupyterLab and install all required dependencies.

This repository contains the deliverables for **Project 2: Reproducibility in Natural Language Processing** for **Statistics 159/259, Fall 2025 at UC Berkeley**. The project focuses on implementing and critically evaluating modern NLP pipelines, from foundational text processing to advanced topic modeling using both traditional (LDA) and state-of-the-art (BERTopic) methods. A key emphasis of the assignment is **reproducibility**, requiring a structured repository, clear documentation, and a deployed MyST site.

Alternatively, you can run the notebooks locally:

1. **Create the conda environment:**
```bash
conda env create -f environment.yml
```

2. **Activate the conda environment**
```bash
conda activate sotu
```

## Repository Structure

```bash
data/
  └─ SOTU.csv           # State of the Union speech dataset

outputs/                # Generated outputs from notebooks, including saved figures     
  └─avg_wordcount_per_president.png
  └─pyLDAvis_interactive.html
  └─speeches_per_president.png
  └─speeches_per_year.png
  └─topic_distribution.html
  └─viz_distribution.html
  └─wordcount_distribution.png
  └─wordcount_over_year.png

nlp-P01.ipynb            # Part 1 — Data loading and exploratory data analysis
nlp-P02.ipynb            # Part 2 — Text processing and TF-IDF vectorization
nlp-P03.ipynb            # Part 3 — Topic modeling using LDA and BERTopic
nlp-P04.ipynb            # Part 4 — Word frequency analysis over time

environment.yml          # Environment configuration file (for reproducibility and Binder)
myst.yml                 # MyST metadata configuration
README.md                # Project overview and instructions
```

## Notes 

- All static and interactive plots generated in Parts 1–4 are saved automatically in the outputs/ folder for reproducibility.
- The project is fully reproducible by running each notebook.
- The environment is specified in environment.yml, so you will need to ensure you have run "conda env create -f environment.yml" to have "sotu" environment ready.
- All required data files are included in the data/ folder.
