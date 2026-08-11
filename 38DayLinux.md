# Title: Processing Structured Data with `awk`

---

## (1) Create `employees.csv` with the columns ID, Name, Department, and Salary. Display only the Name column using awk.

### Ans:

```bash
nano employees.csv
```

Example content:

```text
ID,Name,Department,Salary
1,Rahul,IT,60000
2,Priya,HR,45000
3,Amit,Sales,55000
```

```bash
awk -F',' '{print $2}' employees.csv
```

---

## (2) Display the Name and Salary columns from `employees.csv`.

### Ans:

```bash
awk -F',' '{print $2, $4}' employees.csv
```

---

## (3) Show only employees whose salary is greater than 50000.

### Ans:

```bash
awk -F',' '$4 > 50000 {print $2, $4}' employees.csv
```

---

## (4) Print only the first line (header) of `employees.csv` using awk.

### Ans:

```bash
awk 'NR==1' employees.csv
```

---

## (5) Display your current working directory after completing today's tasks.

### Ans:

```bash
pwd
```
