# Usage Guide

## Running the notebook
Open `notebooks/fake_news_colab_notebook.ipynb` in Jupyter or Colab.

## Running as scripts
1. Ensure `data/train.csv` and `data/test.csv` exist.
2. Preprocess:
    ```bash
    python src/preprocess.py --input data/train.csv --output data/train_clean.csv
    ```
3. Train:
    ```bash
    python src/train.py --data data/train_clean.csv --model-dir models/
    ```
4. Evaluate:
    ```bash
    python src/evaluate.py --data data/test_clean.csv --model-dir models/
    ```
