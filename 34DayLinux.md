# Title: Extracting Columns with `cut`

---

## (1) Create `employees.csv` with the columns ID, Name, Department, and Salary. Display only the Name column.

### Ans:

```bash
nano employees.csv
```

(Type data, save and exit.)

```bash
cut -d ',' -f2 employees.csv
```

---

## (2) Display the Name and Department columns together from `employees.csv`.

### Ans:

```bash
cut -d ',' -f2,3 employees.csv
```

---

## (3) Create `products.csv` with four columns. Display only the first and fourth columns.

### Ans:

```bash
nano products.csv
```

(Type data, save and exit.)

```bash
cut -d ',' -f1,4 products.csv
```

---

## (4) Create `notes.txt` with one line of text. Display only the first 10 characters using `cut`.

### Ans:

```bash
nano notes.txt
```

(Type one line, save and exit.)

```bash
cut -c1-10 notes.txt
```

---

## (5) Display your current working directory after completing today's tasks.

### Ans:

```bash
pwd
```
