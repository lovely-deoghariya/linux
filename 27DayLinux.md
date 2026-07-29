# Title: Revision Quiz #3 - Finding Files & Searching Text

---

## (1) Create a folder named `revision3` with subfolders `data`, `logs`, and `scripts`. Inside them create `employees.csv`, `sales.csv`, `app.log`, and `run.sh`. Use `find` to locate `employees.csv`.

### Ans:

```bash
mkdir revision3
cd revision3
mkdir data logs scripts
touch data/employees.csv data/sales.csv logs/app.log scripts/run.sh
find . -name "employees.csv"
```

---

## (2) Add the words `INFO`, `WARNING`, and `ERROR` to `app.log` using Nano. Use `grep` to display only the line containing `ERROR`.

### Ans:

```bash
nano logs/app.log
```

(Add the words, then save and exit.)

```bash
grep "ERROR" logs/app.log
```

---

## (3) Use a wildcard to list only all `.csv` files inside the `revision3` project.

### Ans:

```bash
ls data/*.csv
```

---

## (4) If `locate` is available on your system, try locating `employees.csv`. If it is not available, explain the difference between `locate` and `find`.

### Ans:

```bash
locate
