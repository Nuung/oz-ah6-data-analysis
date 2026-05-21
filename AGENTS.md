# AGENTS.md

## Project Context

This repository contains all materials for the online course **"Python을 활용한 헬스케어 데이터 분석 및 시각화"**.

- Course format: online live lecture materials and exercises.
- Duration: **3 days**.
- Live lecture time: **10:00–15:00 KST** each day.
- Main audience: learners practicing healthcare data analysis and visualization with Python.
- Primary materials include Jupyter notebooks, slides, PDFs, datasets, and practice assignments.

When modifying or adding content, preserve the course-oriented structure: examples should be understandable for learners, reproducible in class, and appropriate for healthcare data analysis education.


## Project Layout

Keep course materials organized by day and purpose:

```text
course/
  day01/
    notebooks/
    assignments/
  day02/
    notebooks/
    assignments/
  day03/
    notebooks/
    assignments/
resources/
  curriculum/
  documents/
  slides/
```

- Put lecture notebooks under `course/dayXX/notebooks/`.
- Put practice or assignment notebooks under `course/dayXX/assignments/`.
- Put curriculum spreadsheets and planning documents under `resources/curriculum/`.
- Put PDF handouts and references under `resources/documents/`.
- Put presentation files under `resources/slides/`.
- Keep the repository root limited to project configuration and top-level documentation.

## Python Version & Typing

- Use **Python 3.13 or higher**.
- Do **not** use the `typing` module for type hints.
- Always use **built-in types** for annotations.
  - Good: `list[str]`, `dict[str, int]`, `tuple[int, ...]`, `int | None`
  - Avoid: `typing.List`, `typing.Dict`, `typing.Tuple`, `typing.Optional`, `typing.Union`
- Keep examples compatible with the repository setting in `.python-version` and `pyproject.toml`.

## Code Style

Follow these style guides:

- Google Python Style Guide: <https://google.github.io/styleguide/pyguide.html>
- PEP 8: <https://peps.python.org/pep-0008/>

If there is any conflict between local conventions and these guides, prefer clarity and consistency within this project.

Additional local conventions:

- Prefer readable, classroom-friendly code over clever abstractions.
- Use descriptive variable names, especially in notebooks and exercises.
- Keep cells and examples focused on one learning objective at a time.
- Avoid adding unnecessary dependencies.
- For notebooks, make outputs reproducible and avoid hidden state assumptions between cells.

## Research & Reference Policy

Actively consult external official materials and high-quality best examples before making substantive educational, analytical, visualization, or API-related changes.

When referencing external material:

- Prefer official documentation first, such as Python, pandas, NumPy, Matplotlib, Seaborn, Plotly, scikit-learn, Jupyter, and relevant public-health or healthcare-data sources.
- Use reputable best-practice examples, but adopt them critically rather than copying them blindly.
- Compare references against this course's learner level, time limits, and healthcare-analysis context.
- Keep examples simple enough for live instruction from **10:00 to 15:00**.
- Cite or link sources when they materially influence explanations, examples, or assignments.

## Educational Content Guidelines

- Explain not only *what* code does, but also *why* each step matters in data analysis.
- Favor realistic healthcare-analysis scenarios while avoiding sensitive or personally identifiable health information.
- Use anonymized, synthetic, or public datasets unless the repository already provides approved materials.
- Make practice assignments self-contained with clear instructions and expected learning outcomes.
- For visualizations, emphasize correct interpretation, readable labels, units, legends, and accessibility-friendly color choices.

## Verification

Before claiming completion:

- Run relevant checks when code files are changed, such as linting, formatting, type checks, tests, or notebook smoke checks where practical.
- For notebook/material edits, verify that examples are internally consistent and can be followed in lecture order.
- Report what was changed and what validation was performed.
