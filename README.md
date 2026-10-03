# DALAS Project
Authors : 
- Melis TAN
- Daria SHTYKA
- Charles DELEMOLLE
## Table of contents

- [Project structure](#project-structure)
<!-- - [Workflow](#workflow) -->
<!-- - [Data conventions](#data-conventions) -->
<!-- - [Deliverables](#deliverables) -->
- [Getting started](#getting-started)

## Project structure

```text
├── README.md                   <- Main project presentation and setup guide
├── requirements.txt            <- Python dependencies (or environment.yml / pyproject.toml)
│
├── data/
│   ├── raw/                    <- Raw data from scraping/APIs (never modify manually)
│   ├── processed/              <- Cleaned data ready for analysis and dashboarding
│   └── README.md               <- Data dictionary (variable definitions, sources)
│
├── src/                        <- Reusable Python scripts / modules
│   ├── __init__.py
│   ├── data_collection.py      <- Scraping and API routines
│   ├── preprocessing.py        <- Data cleaning and transformation functions
│   └── utils.py                <- Visualization or helper functions
│
├── notebooks/                  <- Exploratory analysis notebooks (ordered by workflow)
│   ├── 01_data_collection.ipynb
│   ├── 02_eda_and_cleaning.ipynb
│   └── 03_analysis.ipynb
│
├── dashboard/                  <- Deliverable 2 (TME 6)
│   ├── app.py                  <- Dashboard entry point (Streamlit / Dash / Shiny)
│   ├── components/             <- Visualizations, layout helpers
│   └── README.md               <- How to run the dashboard locally
│
└── deliverables/
    ├── TME4_research_question/ <- Deliverable 1
    │   └── report.pdf          <- 2-page report on dataset & questions
    │
    ├── TME6_dashboard/         <- Deliverable 2 notes/links
    │   └── instructions.md
    │
    └── TME9_final_report/      <- Deliverable 3
        ├── visual_report.pdf   <- Main visual report (max 12 pages / 2500 words)
        ├── technical_report.pdf<- Technical report (data prep, decisions, hyperparams)
        └── src_report/         <- LaTeX sources or HTML generation files (if applicable)
```

<!-- ## Workflow

The project follows this general workflow:

1. Collect data using the scripts in `src/data_collection.py`.
2. Keep untouched source files in `data/raw/`.
3. Clean and transform the data with `src/preprocessing.py`.
4. Save analysis-ready data in `data/processed/`.
5. Explore and analyse the data in the numbered notebooks.
6. Build and run the dashboard from `dashboard/app.py`.
7. Store final reports and supporting material in `deliverables/`.

## Data conventions

- Do not edit files in `data/raw/` manually.
- Document datasets, variables, sources, and transformations in
  `data/README.md`.
- Keep notebooks ordered according to the analysis workflow.
- Put reusable logic in `src/` rather than duplicating it in notebooks.
- Keep dashboard-specific instructions in `dashboard/README.md`.

## Deliverables

### TME 4 — Research question

The research question deliverable contains the dataset description and the
questions guiding the analysis.

### TME 6 — Dashboard

The dashboard deliverable contains the interactive visualisation and the
instructions required to run it locally.

### TME 9 — Final report

The final deliverable contains:

- a visual report of up to 12 pages and 2,500 words;
- a technical report describing data preparation, decisions, and
  hyperparameters;
- the source files used to generate the reports, when applicable. -->

## Getting started

Install the dependencies with `pip install -r requirements.txt`, then follow the
instructions in the relevant component:

- use the notebooks for exploratory analysis;
- see `dashboard/README.md` for dashboard instructions;
- see `data/README.md` for the data dictionary and data sources.

Freeze the new requirements after your work with `pip freeze > requirements.txt`
