<h1 align="center">📊 Data Formats Lab</h1>
<h3 align="center">CSV vs JSON vs Parquet with Python</h3>

<p align="center">
  A hands-on comparison of the three most common data formats in analytics and data engineering: how they store data, how they behave, and how to validate them.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.9+-3776AB?logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/Pandas-150458?logo=pandas&logoColor=white" alt="Pandas">
  <img src="https://img.shields.io/badge/NumPy-013243?logo=numpy&logoColor=white" alt="NumPy">
  <img src="https://img.shields.io/badge/PyArrow-Parquet-orange" alt="PyArrow">
  <img src="https://img.shields.io/badge/Jupyter-F37626?logo=jupyter&logoColor=white" alt="Jupyter">
</p>

---

## 🎯 Overview

Data moves between systems as files, and the format you choose affects **storage size, speed, and data integrity**. This project takes one `orders` dataset, saves it as CSV, JSON, and Parquet, reloads each file, and compares the results.

The goal is not just to read and write files, but to **verify that data survives a round trip** unchanged.

## 🔍 What This Project Covers

| Format | What I Practiced |
|--------|------------------|
| **CSV** | Reading and writing with Pandas, inspecting rows, columns, and dtypes |
| **JSON** | Objects and arrays, the `json` module, `pd.read_json()`, flattening nested data with `pd.json_normalize()` |
| **Parquet** | Columnar storage, reading and writing with PyArrow, comparing file size and dtypes |
| **Validation** | Comparing data before and after save/load, checking dtypes and consistency |

## 📈 Results

> Replace the placeholders with your own measured values.

| Format | File Size | Dtypes Preserved? | Notes |
|--------|-----------|-------------------|-------|
| CSV | `X MB` | ❌ Partially | e.g. dates reload as strings |
| JSON | `X MB` | ❌ Partially | Good for nested data, larger on disk |
| Parquet | `Y MB` | ✅ Yes | Compact, columnar, typed |

## 💡 Key Takeaways

- **CSV** is simple and universally supported, but data types must be handled explicitly.
- **JSON** fits nested and semi-structured data, especially API responses.
- **Parquet** is built for analytics: columnar, compressed, and type-aware.
- **Never assume** data is correct after saving and loading. Validate it.

## 🗂️ Project Structure

```text
data-formats-lab/
├── csv_json_parquet.ipynb   # Main notebook with all experiments
├── orders.csv               # Sample data (CSV)
├── orders.json              # Sample data (JSON)
├── orders.parquet           # Sample data (Parquet)
└── README.md
```

## 🚀 Getting Started

```bash
# 1. Clone the repository
git clone https://github.com/Bilvish/data-formats-lab.git
cd data-formats-lab

# 2. Install dependencies
pip install pandas numpy pyarrow jupyter

# 3. Launch the notebook
jupyter notebook csv_json_parquet.ipynb
```

Run the cells from top to bottom to reproduce every experiment.

## 🛠️ Tech Stack

Python · Pandas · NumPy · PyArrow · Jupyter Notebook

## 🔭 Next Steps

- [ ] Benchmark read and write speed on larger datasets
- [ ] Compare compression codecs (Snappy, Gzip) for Parquet
- [ ] Explore partitioned Parquet datasets
- [ ] Add schema validation checks

## 👤 Author

**Bilvish**
🔗 [GitHub](https://github.com/Bilvish)

*Part of my journey toward a career in Data Engineering. Feedback and suggestions are welcome.*