# Auto String Encoder

[![Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue)](https://www.python.org/)

A lightweight python utility designed to automate the routine task of converting text and categorical variables into integer format for machine learning models. The function automatically scans the data and performs in-place transformations to optimize memory usage.

---

## Features

* **Automatic Target Selection:** Scans the entire DataFrame and automatically filters out only `object` and `string` data types.
* **In-Place Modification:** Modifies the source DataFrame directly without duplicating data in memory.
* **Encoder Tracking:** Saves and returns every fitted `LabelEncoder` instance in a dictionary, allowing for future mapping and inverse transformations (`inverse_transform`).

---

## Installation & Dependencies

Ensure you have `pandas` and `scikit-learn` installed:

```bash
pip install pandas scikit-learn
