# MLwPython-Decision-Trees-test
This project uses supervised machine learning to classify penguin species from the Palmer Penguins dataset. It demonstrates a complete end‑to‑end workflow: data cleaning, exploratory data analysis (EDA), model building, and evaluation.

## Project Summary

The goal of this project is to predict the species of a penguin — **Adelie, Gentoo, or Chinstrap** — using physical measurements such as bill length, bill depth, flipper length, and body mass.

The [notebook](https://github.com/Lance-Cruz/MLwPython-Decision-Trees-test/blob/main/LanceCruz_MLwithPythonProject.ipynb) walks through:
* Loading and inspecting the dataset
* Cleaning missing or inconsistent values
* Visualising relationships between features
* Training a Decision Tree Classifier
* Evaluating accuracy and model behaviour

## Models Used
This project uses a Decision Tree Classifier from [scikit‑learn](https://scikit-learn.org/stable/index.html) to predict penguin species based on their physical measurements. The notebook applies several machine learning and data analysis techniques, including:

* Train/Test Split — dividing the dataset to evaluate model performance

* Data Visualisation using:
    * Pie charts (species distribution)
    * Histograms (feature distributions)
    * Box plots (feature comparison across species)

* Correlation Analysis — identifying relationships between numerical features

* Decision Tree Training — fitting the model on physical measurements

* Confusion Matrix — evaluating classification accuracy and misclassifications

## How to run the Notebook (Google Colab)
This notebook currently imports the dataset directly from the raw CSV hosted in this GitHub repository, so no manual file upload is required.

However, if any issues occur with remote loading (e.g., network errors, GitHub rate limits), you can fall back to using the local [`penguins.csv`](https://github.com/Lance-Cruz/MLwPython-Decision-Trees-test/blob/main/penguins.csv) file included in this repository.

**Option 1 — Normally**\
The notebook loads the dataset using the raw GitHub URL, so you can simply run all cells without additional setup.

**Option 2 — Manual Import**\
If the automatic import fails:

1.  Download `penguins.csv` from this repository
2.  Upload it to your Google Drive.
3.  Mount Google Drive in Colab:
    ```python
    from google.colab import drive
    drive.mount('/content/drive')
    ```
4.  Update the file path in the notebook to point to the location of `penguins.csv` in your Drive.
5.  Run all cells sequentially to execute to the full machine learning workflow.
