# 📊 Data Analytics Environment Setup (Python + Jupyter + Conda)

This guide helps you set up a clean data analytics project using **Anaconda**, **Jupyter Notebook**, and **virtual environments**. Follow this to replicate the environment structure for any future projects.

---

## 📁 Folder Structure

Create your project folder (e.g., `Data_Analytics`) and inside it:

```
Data_Analytics/
├── notebooks/   # Jupyter notebooks go here
└── data/        # Datasets go here
```

---

## 🔧 Step-by-Step Setup Instructions

### 1. Create Project Folder

Place your project where it is backed up (e.g., OneDrive):

```bash
cd ~/OneDrive
mkdir Data_Analytics
cd Data_Analytics
mkdir notebooks data
```

---

### 2. Create Conda Environment

Create a new Python 3.10 environment (recommended for compatibility):

```bash
conda create --name data_viz_venv python=3.10
```

---

### 3. Activate the Environment

```bash
conda activate data_viz_venv
```

---

### 4. Install Required Packages

```bash
pip install pandas numpy matplotlib seaborn jupyter
pip install plotly scikit-learn openpyxl
```

---

### 5. Download Dataset

Example using Titanic dataset:

```bash
cd data
curl -O https://raw.githubusercontent.com/datasciencedojo/datasets/master/titanic.csv
cd ..
```

---

### 6. Register Jupyter Kernel

Register your conda environment so it shows in Jupyter:

```bash
python -m ipykernel install --user --name=data_viz_venv --display-name "Python (data_viz_venv)"
```

---

### 7. Launch Jupyter Notebook

From the `Data_Analytics` directory:

```bash
jupyter notebook
```

Navigate to `notebooks/` → click **New > Python (data_viz_venv)**

---

## ✅ You're Ready!

Your environment is now isolated, reproducible, and organized — ideal for academic and industry-level data science work.

