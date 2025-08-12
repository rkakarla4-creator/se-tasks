
# Quadratic Weather Modeling

This project models temperature variation over time using a quadratic equation of the form:

$$
T(t) = a t^2 + b t + c
$$

where:

* **t** is the time (in days, hours, etc.)
* **a, b, c** are coefficients loaded from a CSV file

## 📂 Files

* **`abc_values_20rows.csv`** – Contains 20 rows of random `a`, `b`, `c` values (each below 10).
* **`weather_model.py`** – The Python script that reads the CSV, computes temperature values, and plots the curves.
* **`weather modeling.ipynb`** – Jupyter Notebook version of the same process.

## ⚙️ Requirements

Install dependencies:

```bash
pip install matplotlib pandas
```

## ▶️ Usage

1. Ensure `abc_values_20rows.csv` is in the same directory as the Python file.
2. Run the script:

```bash
python weather_model.py
```

3. The script will:

   * Read coefficients `a, b, c` from the CSV
   * Compute temperature over 0–10 time units for each row
   * Plot each curve with a unique color and legend label

## 📊 Output

The program will display a line plot where:

* **X-axis** → Time (0–10)
* **Y-axis** → Calculated Temperature
* Each curve represents one set of `(a, b, c)` coefficients.


