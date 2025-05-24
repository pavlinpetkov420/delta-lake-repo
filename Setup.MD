
# 🔧 Local Setup Guide

This guide walks you through setting up a local development environment for running Delta Lake experiments using PySpark and JupyterLab.

---

## ✅ Prerequisites

Ensure you have the following installed:

- **Python** 3.8 or higher  
- **Java** 8, 11 or (required by Spark)  
- **pip** – Python package manager  
- **Git** – for cloning this repository  
- Optional: [JupyterLab][jupyterlab]

---

## 📁 1. Clone the Repository

```bash
git clone https://github.com/your-username/delta-lake-repo.git
cd delta-lake-experiments
```

---

## 🐍 2. Create a Python Virtual Environment

Create and activate a virtual environment:

**Unix/macOS**:

```bash
python -m venv venv
source venv/bin/activate
pip install --upgrade pip
```

**Windows**:

```cmd
python -m venv venv
venv\Scripts\activate
pip install --upgrade pip
```

---

## 📦 3. Install Python Dependencies

Install required packages:

```bash
pip install -r requirements.txt
```

If you want to create `requirements.txt` manually, here is an example:

```
pyspark==3.5.4
delta-spark==3.2.0
jupyterlab
```

> ⚠️ You do not need to manually download any JAR files. The `delta-spark` package automatically includes Delta Lake JARs.

---

## 🔥 4. Initialize Spark Session for Delta Lake

Use the following Python code to start a Spark session configured for Delta Lake:

- Open IntializeSparkSession.ipynb
- Add your path to JAR file
- Add your path for spark-warehouse
- Do any other updates, if necessary

---

## 🚀 5. Launch JupyterLab

Start JupyterLab with the command:

```bash
jupyter lab
```

Open your browser and navigate to [http://localhost:8888](http://localhost:8888) to access the notebooks.

---

## 📎 Notes

- This repository is **only for educational and testing purposes**.  
- If you run into Java-related errors, check that your `JAVA_HOME` environment variable points to a valid Java installation.

---

## 📚 Related Resources

- [Delta Lake: The Definitive Guide (Free PDF)][book-pdf]  
- [delta-spark on PyPI][delta-spark]  
- [Apache Spark Documentation][spark-docs]  
- [JupyterLab Documentation][jupyterlab]

---

[book-pdf]: https://delta.io/pdfs/dldg_databricks.pdf  
[delta-spark]: https://pypi.org/project/delta-spark/  
[spark-docs]: https://spark.apache.org/docs/latest/  
[jupyterlab]: https://jupyterlab.readthedocs.io/
