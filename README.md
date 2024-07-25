
# MultiRC Dataset Analysis and Model Building

This repository contains a comprehensive Jupyter Notebook for analyzing the MultiRC (Multi-Sentence Reading Comprehension) dataset. The notebook includes data loading, preprocessing, exploratory data analysis, feature engineering using TF-IDF, model building with Logistic Regression and BERT, model evaluation, and interpretability using LIME.

## Table of Contents

- [MultiRC Dataset Analysis and Model Building](#multirc-dataset-analysis-and-model-building)
  - [Table of Contents](#table-of-contents)
  - [Introduction](#introduction)
  - [Dataset](#dataset)
  - [Notebook Overview](#notebook-overview)
  - [Requirements](#requirements)
  - [Installation](#installation)
  - [Usage](#usage)
  - [Results](#results)
  - [Future Work](#future-work)
  - [Contributing](#contributing)
  - [License](#license)

## Introduction

MultiRC (Multi-Sentence Reading Comprehension) is a dataset of short paragraphs and multi-sentence questions that can be answered from the content of the paragraph. The dataset poses several challenges:
1. The number of correct answer-options for each question is not pre-specified.
2. The correct answer(s) is not required to be a span in the text.
3. The paragraphs have diverse provenance, extracted from different domains such as news, fiction, historical text, etc.

The goal of this dataset is to encourage the research community to explore approaches that go beyond sophisticated lexical-level matching.

## Dataset

The MultiRC dataset can be found [here](https://cogcomp.seas.upenn.edu/multirc/).

## Notebook Overview

The notebook, `MultiRC_NLP_Analysis.ipynb`, includes the following sections:

1. **Data Loading:** Load the dataset from JSON files.
2. **Data Preprocessing:** Clean and preprocess the text data.
3. **Exploratory Data Analysis (EDA):** Analyze the distribution of the number of questions per paragraph and the class distribution.
4. **Feature Engineering:** Use TF-IDF for feature extraction.
5. **Model Building:**
   - Logistic Regression
   - BERT for Sequence Classification
6. **Model Evaluation:** Evaluate the models using accuracy and classification report.
7. **Interpretability:** Use LIME for model interpretability.

## Requirements

The following Python libraries are required to run the notebook:

- pandas
- matplotlib
- seaborn
- scikit-learn
- transformers
- torch
- lime

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/debjit-mandal/multirc-nlp-analysis.git
    cd multirc-nlp-analysis
    ```

2. Install the required libraries:
    ```bash
    pip install pandas matplotlib seaborn scikit-learn transformers torch lime
    ```

## Usage

1. Navigate to the cloned repository directory.
2. Launch Jupyter Notebook:
    ```bash
    jupyter notebook
    ```
3. Open the `MultiRC_NLP_Analysis.ipynb` notebook and run the cells sequentially.

## Results

The notebook provides detailed analysis and results for the MultiRC dataset. It includes visualizations for EDA, performance metrics for the models, and interpretability insights using LIME.

## Future Work

Future improvements could involve:
- Experimenting with other NLP models.
- Improving preprocessing techniques.
- Exploring more advanced interpretability methods.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
