# Title: Module 4 Practical Workflow & Review - Text Processing

---

## (1) Create `employees.csv` with the columns ID, Name, Department, Salary and at least 10 records. Use `wc -l` to count the total lines.

### Ans:

```bash
nano employees.csv
```

Example:

```text
ID,Name,Department,Salary
1,Rahul,IT,65000
2,Priya,HR,45000
3,Amit,Sales,70000
4,Neha,IT,62000
5,Rohan,Finance,55000
6,Anjali,HR,72000
7,Vikas,Sales,68000
8,Pooja,IT,59000
9,Karan,Finance,80000
10,Meena,HR,61000
```

```bash
wc -l employees.csv
```

---

## (2) Extract the Name and Salary columns using `cut`. Then use `awk` to display only employees whose salary is greater than 60000.

### Ans:

```bash
cut -d',' -f2,4 employees.csv
```

```bash
awk -F',' '$4 > 60000 {print $2, $4}' employees.csv
```

---

## (3) Create `departments.txt` with duplicate department names. Use `sort` and `uniq -c` to count how many times each department appears.

### Ans:

```bash
nano departments.txt
```

Example:

```text
IT
HR
IT
Sales
Finance
HR
IT
Sales
HR
```

```bash
sort departments.txt | uniq -c
```

---

## (4) Create `first_names.txt` and `last_names.txt`. Merge them into `full_names.csv` using `paste` with a comma delimiter. Convert the merged output to uppercase using `tr` and save it as `full_names_upper.csv`.

### Ans:

```bash
nano first_names.txt
```

```text
Rahul
Priya
Amit
```

```bash
nano last_names.txt
```

```text
Sharma
Singh
Kumar
```
