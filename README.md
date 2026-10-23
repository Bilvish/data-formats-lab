# 📊 Data Formats Lab: CSV vs JSON vs Parquet

A hands-on Python project exploring how CSV, JSON, and Parquet store data, preserve data types, and support data analytics and engineering workflows.

## 🎯 Overview

This project uses an orders dataset to practice writing, reading, and validating data in three common formats. The goal is to understand their differences and verify data consistency after saving and reloading files.

## 🛠️ Tech Stack

- Python
- Pandas
- NumPy
- PyArrow
- Jupyter Notebook

## 📚 What I Learned

### CSV
- Reading and writing tabular data with Pandas
- Inspecting rows, columns, and data types
- Understanding data type inference when loading CSV files

### JSON
- Working with JSON objects and arrays
- Reading and writing JSON using Python
- Loading JSON with Pandas
- Exploring nested data with `pd.json_normalize()`

### Parquet
- Reading and writing Parquet files with PyArrow
- Understanding columnar storage
- Comparing file sizes and data types across formats

### Data Validation
- Comparing data before and after saving and loading
- Checking data types and data consistency
- Understanding why different formats may behave differently during round trips

## 🗂️ Project Structure

```text
data-formats-lab/
├── csv_json_parquet.ipynb
├── nested_order.json
├── order.json
├── orders.csv
├── orders.json
├── orders.parquet
└── README.md
```

## 🚀 Getting Started

Clone the repository:

```bash
git clone https://github.com/Bilvish/data-formats-lab.git
cd data-formats-lab
```

Install the required libraries:

```bash
pip install pandas numpy pyarrow jupyter
```

Launch the notebook:

```bash
jupyter notebook csv_json_parquet.ipynb
```

Run the notebook cells from top to bottom.

## 💡 Key Takeaways

- CSV is simple and widely supported, but data types may need explicit handling.
- JSON supports structured and nested data.
- Parquet is a columnar format well suited to analytical workloads.
- Data should be validated after saving and loading instead of assuming the round trip succeeded.

## 🔭 Future Improvements

- Benchmark read and write times
- Compare Parquet compression options
- Explore partitioned Parquet datasets
- Add automated schema validation

## 👤 Author

**Bilvish**

[GitHub Profile](https://github.com/Bilvish)

*Part of my learning journey toward Data Engineering.*
