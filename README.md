# Auto Preprocessing Toolkit

[![Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue)](https://www.python.org/)

A lightweight and efficient utility designed to automate routine data preprocessing tasks for machine learning pipelines. This tool focuses on automatic handling of missing values and smart in-place encoding of categorical text variables directly within pandas DataFrames.

---

## Features

* **In-Place Categorical Encoding (`auto_encode`):** Detects all object and string columns, converts them to valid strings, and encodes them into integers using `LabelEncoder`. The modifications are applied directly to the original DataFrame to save operational memory. Returns a dictionary containing all fitted encoder objects for future inverse transformations.
* **Smart Missing Value Imputation (`fill_none`):** Automatically determines column data types to apply optimal missing data strategies. Text columns are filled using the mode or a fallback token. Numerical columns are imputed using the median to stay robust against outliers.

---

## Installation & Dependencies

Ensure you have `pandas` and `scikit-learn` installed in your environment:

```bash
pip install pandas scikit-learn
