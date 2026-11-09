# ML6402 – Machine Learning Practicals

Al-Quds Open University  
Master in Information Technology – Information Technology and Communication  
Instructor: **Dr. Ahmed Sabbah**

This repository contains practical Jupyter notebooks, datasets, and exercises for **ML6402 – Machine Learning**.

## Practical approach

Each practical follows the same learning pattern:

**Concept → Dataset → Guided Implementation → Interpretation → Student Exercise → Challenge**

The notebooks are designed to run either:

- locally with **Anaconda / Jupyter Notebook**, or
- online with **Google Colab**.

## Course practical structure

| Week | Topic | Practical status |
|---|---|---|
| 01 | Overview of Machine Learning | Available |
| 02 | Python for Machine Learning | Available |
| 03 | Data Pre-processing | Available |
| 04 | Simple Linear Regression | Available |
| 05 | Multiple and Polynomial Regression | Available |
| 06 | Classification I | Available |
| 07 | Classification II and Evaluation | Available |
| 08 | Support Vector Machines and Classifier Implementation | Available |
| 09 | Clustering | Available |
| 10 | Association Mining | Available |
| 11 | Artificial Neural Networks | Available |
| 12 | Deep Learning and CNNs | Available |
| 13 | RNNs and LSTMs | Available |
| 14 | Model Evaluation and Experimental Practice | Available |
| 15 | ML Research: From Experiment to Paper | Available |
| 16 | Course Integration / Research Presentations | Available |

---

## Dataset loading convention

Every practical that uses a CSV dataset follows the same rule:

1. Try the local lecture folder:
   `data/<dataset>.csv`
2. Try the repository-relative path:
   `LectureXX_.../data/<dataset>.csv`
3. If the file is not available locally, load the same dataset from the raw GitHub URL.

This makes the same notebook usable in:

- a cloned local repository;
- Jupyter started from the repository root;
- Jupyter started inside the lecture folder;
- Google Colab.

The notebook prints the source it used, for example:

```text
Loaded from: data/50_AdAgency.csv
```

or:

```text
Loaded from: https://raw.githubusercontent.com/asabbah44/ML6402-Machine-Learning-Practicals/main/...
```

Lectures that use datasets bundled with Scikit-Learn do not require external paths.

---

# Option 1 – Run locally with Anaconda / Jupyter

## Step 1 – Clone the repository

```bash
git clone https://github.com/asabbah44/ML6402-Machine-Learning-Practicals.git
cd ML6402-Machine-Learning-Practicals
```

## Step 2 – Create the environment

```bash
conda env create -f environment.yml
```

## Step 3 – Activate it

```bash
conda activate ml6402
```

## Step 4 – Start Jupyter

```bash
jupyter notebook
```

Run each notebook from top to bottom.

To download later updates:

```bash
git pull
```

---

# Option 2 – Run with Google Colab

1. Open Google Colab.
2. Choose **File → Open notebook**.
3. Select the **GitHub** tab.
4. Enter:

```text
asabbah44/ML6402-Machine-Learning-Practicals
```

5. Open the required notebook.

For notebooks that use CSV files, the local file will usually not exist in a standalone Colab session. The loader therefore uses the raw GitHub dataset automatically.

---

## Main source alignment

Where relevant, the practicals adapt datasets and implementation ideas from the course copy of Parteek Bhatia's *Machine Learning with Python* companion materials:

```text
https://github.com/asabbah44/ml_with_python
```

The material is reorganized for the ML6402 course and emphasizes:

- reproducibility;
- interpretation;
- train/test separation;
- avoiding data leakage;
- appropriate evaluation metrics;
- experimental practice.

## Additional packages

Most practicals use NumPy, Pandas, Matplotlib, and Scikit-Learn.

The following topics require additional packages:

- **Association Mining:** `mlxtend`
- **CNN / RNN / LSTM:** `tensorflow`

Both are included in `requirements.txt` and `environment.yml`.
