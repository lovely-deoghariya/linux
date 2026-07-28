# Title: Real-World Data Engineering Search Practice

---

## (1) Create a folder named `retail_project` with subfolders `data`, `logs`, and `scripts`. Inside `data` create `employees.csv`, `customers.csv`, and `sales.csv`.

### Ans:

```bash
mkdir retail_project
cd retail_project
mkdir data logs scripts
touch data/employees.csv data/customers.csv data/sales.csv
```

---

## (2) Using Nano, add at least 5 rows of sample data to `employees.csv`. Use `find` to locate `employees.csv`.

### Ans:

```bash
nano data/employees.csv
```

(Add at least 5 rows, then save and exit.)

```bash
find . -name "employees.csv"
```

---

## (3) Create `application.log` inside the `logs` folder. Add the word `ERROR` on one line and `INFO` on another. Use `grep` to search for `ERROR`.

### Ans:

```bash
nano logs/application.log
```

(Add `ERROR` and `INFO`, then save and exit.)

```bash
grep "ERROR" logs/application.log
```

---

## (4) Use a wildcard to list only all `.csv` files inside the `data` folder.

### Ans:

```bash
ls data/*.csv
```

---

## (5) Display your current working directory and list every directory inside `retail_project`.

### Ans:

```bash
pwd
ls -d */
```
