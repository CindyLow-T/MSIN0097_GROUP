# Hotel Booking Cancellation Benchmark

## Repository Scope
This repository contains benchmark artifacts for agent-assisted data science workflows on a shared hotel booking dataset.

Current workflow scope:
- Task 1: Dataset ingestion, schema checks, preprocessing design
- Task 2: Exploratory data analysis
- Task 3: Baseline modelling pipeline
- Task 4: Structured model improvement and focused tuning

---

## Data
Files used in this repository:
- `hotel_bookings.xlsx`
- `dataset description.pdf`

Rules:
- Use only the provided dataset and documentation.
- Do not introduce external datasets.

---

## Notebooks
- `Predictive Codex.ipynb`
- `Predictive Claude.ipynb`
- `Predictive Cursor.ipynb`

Each notebook should be executable top-to-bottom.

---

## Standard Workflow Protocol
For each task section, follow this structure:
1. Plan
2. Risks
3. Implementation
4. Verification
5. Revised final answer

---

## Methodological Rules
- Define target and feature scope explicitly.
- Apply train/test split before preprocessing or model fitting.
- Fit preprocessing on training data only.
- Exclude leakage-prone post-outcome variables.
- Keep candidate model comparison on training data only.
- Use the test set only for final evaluation.
- Keep all steps reproducible (fixed seeds, explicit pipelines, auditable code).

---

## Fairness and Reproducibility Constraints
- Use consistent split logic within each notebook workflow.
- Compare candidate models under identical evaluation conditions.
- Report both performance metrics and train-test gap diagnostics.
- Avoid uncontrolled random trial-and-error.
- Keep task order intact; do not rewrite earlier completed task sections.

---

## Suggested Environment
- Python 3.10+
- Jupyter Notebook
- Core libraries: `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`, `pypdf`

---

## Execution
1. Open a notebook.
2. Run all cells in order.
3. Ensure data files are accessible from the configured paths.
4. Do not skip validation and verification cells.
