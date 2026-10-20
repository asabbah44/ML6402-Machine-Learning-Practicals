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
| 01 | Overview of Machine Learning | Planned |
| 02 | Python for Machine Learning | Planned |
| 03 | Data Pre-processing | Available |
| 04 | Simple Linear Regression | Planned |
| 05 | Multiple and Polynomial Regression | Planned |
| 06 | Classification I | Planned |
| 07 | Classification II and Evaluation | Planned |
| 08 | Support Vector Machines and Classifier Implementation | Planned |
| 09 | Clustering | Planned |
| 10 | Association Mining | Planned |
| 11 | Artificial Neural Networks | Planned |
| 12 | Deep Learning and CNNs | Planned |
| 13 | RNNs and LSTMs | Planned |
| 14 | Model Evaluation and Experimental Practice | Planned |
| 15 | ML Research: From Experiment to Paper | Planned |
| 16 | Course Integration / Research Presentations | Planned |

---

# Option 1 – Run locally with Anaconda / Jupyter

This option is recommended if you want the complete repository, datasets, and notebooks on your own computer.

## Step 1 – Install Anaconda

Install **Anaconda Distribution** from the official Anaconda website.

After installation, open:

**Anaconda Prompt**

on Windows.

## Step 2 – Download or clone the repository

### Method A – Using Git

In Anaconda Prompt, run:

```bash
git clone https://github.com/asabbah44/ML6402-Machine-Learning-Practicals.git
```

Then enter the repository:

```bash
cd ML6402-Machine-Learning-Practicals
```

### Method B – Download ZIP

If Git is not installed:

1. Open this repository on GitHub.
2. Click **Code**.
3. Select **Download ZIP**.
4. Extract the ZIP file.
5. Open **Anaconda Prompt**.
6. Change directory to the extracted repository folder.

For example:

```bash
cd C:\Users\YourName\Downloads\ML6402-Machine-Learning-Practicals
```

## Step 3 – Create the ML6402 environment

Run:

```bash
conda env create -f environment.yml
```

This creates an environment called:

```text
ml6402
```

with the main packages used in the course, including:

- Python
- NumPy
- Pandas
- Matplotlib
- Scikit-Learn
- Jupyter Notebook

You normally need to create this environment only once.

## Step 4 – Activate the environment

Each time you want to work on the practicals, open Anaconda Prompt and run:

```bash
conda activate ml6402
```

You should then see something similar to:

```text
(ml6402) C:\...
```

## Step 5 – Start Jupyter Notebook

Run:

```bash
jupyter notebook
```

A browser window should open automatically.

Navigate to the required lecture folder.

For Lecture 3, open:

```text
Lecture03_Data_Preprocessing
```

and then:

```text
ML6402_Practical03_Data_Preprocessing.ipynb
```

## Step 6 – Run the notebook

Inside Jupyter Notebook:

- click a cell;
- press **Shift + Enter** to run it;
- execute the notebook from top to bottom.

The notebook uses the dataset stored in:

```text
Lecture03_Data_Preprocessing/data/
```

So when using the complete repository locally, keep the notebook and its `data` folder in their original locations.

## Updating the repository later

If you cloned the repository using Git, new practicals can be downloaded with:

```bash
git pull
```

Run this from inside the repository folder.

---

# Option 2 – Run online with Google Colab

Google Colab allows you to run Jupyter notebooks in the browser without installing Anaconda or Python locally.

## Method A – Open the notebook through Colab

1. Open **Google Colab**.
2. Choose **File → Open notebook**.
3. Select the **GitHub** tab.
4. Enter:

```text
asabbah44/ML6402-Machine-Learning-Practicals
```

5. Select the required notebook.

For Lecture 3, select:

```text
Lecture03_Data_Preprocessing/ML6402_Practical03_Data_Preprocessing.ipynb
```

6. Run the notebook cells using **Shift + Enter** or the play button beside each cell.

## Method B – Open from GitHub

You may also:

1. open the notebook file in this GitHub repository;
2. copy its GitHub URL;
3. open Google Colab;
4. choose **File → Open notebook → GitHub**;
5. paste the URL and open the notebook.

## Important note about datasets in Colab

When running locally, the notebook can directly access files stored in its `data` folder.

When opening only a notebook in Google Colab, the repository files are not always downloaded automatically.

Therefore, practical notebooks may include code that loads the required dataset directly from this GitHub repository when a local file is not available.

This allows the same notebook to work in both environments:

- **Anaconda/Jupyter** → use the local dataset;
- **Google Colab** → load the dataset from GitHub.

If a notebook reports that a dataset cannot be found in Colab, check the notebook instructions before continuing.

---

# Recommended workflow for students

For the easiest start:

**Google Colab**
- no installation required;
- useful for quickly running exercises;
- good for computers where students cannot install software.

For regular course work:

**Anaconda / Jupyter**
- keeps notebooks and datasets locally;
- provides a stable course environment;
- useful for larger experiments and research work.

Both environments use the same Python code and the same lecture notebooks.

---

# Current practical

The first complete practical is:

```text
Lecture03_Data_Preprocessing/
├── ML6402_Practical03_Data_Preprocessing.ipynb
├── README.md
└── data/
    └── salary.csv
```

Students should first read the Markdown explanation in the notebook, then execute the code cells in order and complete the exercises at the end.

## Notes

The practical materials are aligned with the ML6402 lectures and emphasize reproducibility, fair evaluation, interpretation, and avoiding data leakage.
