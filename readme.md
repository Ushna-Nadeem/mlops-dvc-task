# MLOps DVC Task

This project demonstrates data versioning and reproducibility using **DVC (Data Version Control)** integrated with Git for tracking data and running experiments efficiently.

---

## 📂 Project Overview

* **Data File Tracked:** `data.csv`
* **Version Control:** Git + DVC
* **Script Executed:** `main.py`

---

## 🧪 Workflow Steps

### 🔹 Step 1: Track Dataset with DVC

```bash
dvc add data.csv
git add data.csv.dvc README.md .gitignore
git commit -m "Track updated data.csv with DVC"
git push origin main
```

---

### 🔹 Step 2: Run Script

```bash
python main.py
```

---

### 🔹 Step 3: View Commit History & Restore Previous Data Version

```bash
git log
git checkout <commit_hash>
dvc pull
```

> This will restore the previous version of `data.csv` tracked by DVC.

---

### 🔹 Step 4: Return to Main Branch

```bash
git checkout main
git pull origin main
```

---

## 🛠 Requirements

* [Git](https://git-scm.com/)
* [DVC](https://dvc.org/doc/install)
* Python (for `main.py`)

---

## ✅ Benefits of DVC

* Efficient **data versioning**
* Lightweight tracking of large files
* Seamless **team collaboration** on data
