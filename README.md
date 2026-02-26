# Supplementary Materials

This repository contains the supplementary materials accompanying the publication: *Measuring Corrective Culture in Hospital Responses to Patient Concerns about Safety and Quality Raised Online*.

---

## Contents

| File / Folder | Description |
|---|---|
| `Notebook (Supplementary Materials A).ipynb` | Jupyter notebook (Supplementary Materials A) containing all analysis code, including manual coding reliability results, LLM-based classifier development, and external validation against NHS England Staff Survey data. |
| `Supplementary Materials A.html` | Static HTML export of the notebook — viewable in any browser without running any code. |
| `Supplementary Materials B.pdf` | Manual codebook for scoring engagement and organisational responses. |
| `final_data/IRRdata.csv` | Inter-rater reliability data from the manual coding rounds (RQ1). |
| `final_data/train_results.csv` | Classifier training results (RQ2). |
| `final_data/test_results.csv` | Classifier evaluation results (RQ2). |
| `final_data/full_dataset.csv` | Full dataset used in the quantitative analysis (RQ3). |

---

## Running the Notebook

### Requirements

- Python 3.13
- The following packages (install via pip):

```
pip install pandas numpy matplotlib seaborn krippendorff pingouin openai pydantic scipy scikit-learn statsmodels
```

### OpenAI API Key

The classifier sections of the notebook call the OpenAI API. To run these sections you must have a valid OpenAI API key set as an environment variable:

```bash
export OPENAI_API_KEY="your-api-key-here"
```

Sections of the notebook that do not call the API (e.g., data loading, inter-rater reliability, statistical analyses) can be run without a key.

> **Note:** If you only want to view the analysis without running any code, open `Supplementary Materials A.html` directly in your browser.
