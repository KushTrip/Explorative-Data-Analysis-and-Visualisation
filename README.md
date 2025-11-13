# Exploratory Data Analysis: WHO Life Expectancy (2000-2015)

**Author:** Kush Tripathi

**Matriculation Number:** 92127552

**Course:** DLBDSEDAV01 – Exploratory Data Analysis and Visualization

**University:** IU International University of Applied Sciences

---

## 1. Project Overview

This repository contains the complete exploratory data analysis (EDA) for **Task 1: Visually Exploring a Data Set** of the IU course DLBDSEDAV01.

The project uses the "Life Expectancy (WHO)" dataset from Kaggle, which covers 193 countries from 2000 to 2015. The goal of this analysis is to explore the dataset's structure, clean the data, and use statistical and visual techniques to uncover the key factors correlated with life expectancy.

The full written report, which details the findings and methodology, was submitted separately. This repository provides the technical Jupyter notebook and the raw data used to generate those findings.

---

## 2. Files in This Repository

* `life_expectancy_data.ipynb`: The main Jupyter Notebook containing all Python code, analysis, and visualizations. This file details the entire EDA process, from data cleaning to iterative plot generation.
* `Life Expectancy Data.csv`: The raw dataset used as the input for the notebook.

---

## 3. How to Run This Project

To review the analysis and reproduce the results, please follow these steps:

### Requirements
The analysis relies on the following core Python libraries:
* `pandas`
* `matplotlib`
* `seaborn`
You will need a Python environment capable of running Jupyter Notebooks (such as Anaconda, VS Code with the Jupyter extension, or Google Colab).
The Fastest way to run this program is to open the `life_expectancy_data.ipynb` in google collab and load the csv dataset in there.

### Instructions for running locally

1.  **Clone or Download the Repository:**
    * Clone this repository to your local machine:
        ```
        git clone https://github.com/KushTrip/Explorative-Data-Analysis-and-Visualisation.git
        ```
    * OR download the ZIP file from GitHub and extract it.

2.  **Install Dependencies:**
    If you do not have the required libraries installed, you can install them via pip in your terminal:
    ```
    pip install pandas matplotlib seaborn
    ```

3.  **Launch Jupyter Notebook:**
    Navigate to the project directory in your terminal and run:
    ```sh
    jupyter notebook
    ```
    This will open the Jupyter environment in your browser.

4.  **Run the Analysis:**
    * Click on the `life_expectancy_data.ipynb` file to open it.
    * To see the results and run the code, you can run the cells sequentially by clicking the "Run" button or by pressing `Shift + Enter`.

---

## 4. Summary of Key Findings

The EDA process documented in the notebook revealed several key insights:

* **Strongest Correlates:** Life expectancy showed strong positive linear correlations with **'Schooling'** (0.7) and **'Income composition of resources'** (0.7). It had strong negative correlations with **'Adult Mortality'** (-0.7) and **'HIV/AIDS'** (-0.6).

* **The Development Gap:** A side-by-side box plot revealed a stark 10-year gap in median life expectancy between 'Developed' (79 years) and 'Developing' (69 years) nations.

* **Non-Linear GDP Relationship:** A key "creative choice" was to apply a **logarithmic scale** to the GDP vs. Life Expectancy scatter plot. This revealed a clear "diminishing returns" pattern, where the impact of GDP on longevity is strongest at lower income levels and flattens out for wealthier nations.

* **Multivariate Insights:** A bubble chart combining GDP, Life Expectancy, Population, and Status visually confirmed that a country's **population size has no clear correlation** with its life expectancy.
