# AG News Classification

A text-classification project that assigns news articles to one of four topics: **Sci/Tech**, **Business**, **Sports**, or **World**. The repository includes a Jupyter notebook and train/test CSV files.

## Results

Evaluation on the provided 4,000-example test set:

| Metric | Score |
| --- | --- |
| Accuracy | **93%** |
| Macro F1-score | **0.93** |
| Weighted F1-score | **0.93** |

### Per-class performance

| Class | Precision | Recall | F1-score | Support |
| --- | --- | --- | --- | --- |
| Sci/Tech | 0.88 | 0.92 | 0.90 | 1,025 |
| Business | 0.91 | 0.87 | 0.89 | 999 |
| Sports | 0.98 | 0.98 | 0.98 | 1,013 |
| World | 0.94 | 0.93 | 0.94 | 963 |

The reported metrics are from the evaluation output provided for this project. The confusion matrix and detailed classification report are available in the model evaluation workflow.

## Tech Stack

- Python
- Jupyter Notebook
- `train.csv` and `test.csv`
- Machine-learning / text-processing libraries used in `AG-News_Model.ipynb`

> The exact estimator and preprocessing steps should be described from the notebook implementation. This README avoids naming a specific model without confirming it from the code.

## Repository Structure

```text
Ag_news/
├── AG-News_Model.ipynb
├── train.csv
├── test.csv
└── .gitignore
```

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/mohammedwaleederfaan-coder/Ag_news.git
cd Ag_news
```

### 2. Create and activate a virtual environment

Windows:

```bash
python -m venv .venv
.venv\Scripts\activate
```

macOS/Linux:

```bash
python -m venv .venv
source .venv/bin/activate
```

### 3. Install the notebook dependencies

The repository currently does not include a `requirements.txt`. Install the packages imported by the notebook in your environment. A typical starting point for a notebook-based ML workflow is:

```bash
python -m pip install jupyter pandas numpy scikit-learn matplotlib seaborn
```

If the notebook imports additional libraries, install those as well.

### 4. Open the notebook

```bash
jupyter notebook AG-News_Model.ipynb
```

Run the notebook cells in order. Confirm the data paths in the notebook point to `train.csv` and `test.csv`.

## Label Mapping

The mapping used in the reported evaluation is:

| Label | Category |
| --- | --- |
| 0   | Sci/Tech |
| 1   | Business |
| 2   | Sports |
| 3   | World |

## Evaluation

The project reports accuracy, precision, recall, F1-score, and a confusion matrix. Accuracy alone can hide differences between categories, so per-class metrics are included for a more complete view.

## Future Improvements

- Add a pinned `requirements.txt` for reproducible setup.
- Document the selected model and preprocessing steps.
- Save the confusion matrix as an image and include it here.
- Add a small prediction example for a custom news headline.

## Author

Mohammed Waleed Erfaan — [GitHub profile](https://github.com/mohammedwaleederfaan-coder)
