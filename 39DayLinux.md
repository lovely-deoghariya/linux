# Title: Practical Assignment - Text Processing Toolkit

---

## (1) Create `employees.csv` with the columns ID, Name, Department, and Salary. Add at least 8 employee records.

### Ans:

```bash
nano employees.csv
```

Example:

```text
ID,Name,Department,Salary
1,Rahul,IT,60000
2,Priya,HR,45000
3,Amit,Sales,55000
4,Neha,IT,70000
5,Rohan,Finance,48000
6,Anjali,HR,52000
7,Vikas,Sales,65000
8,Pooja,IT,58000
```

---

## (2) Use `cut` to display the Name and Department columns. Then use `awk` to display employees whose Salary is greater than 50000.

### Ans:

```bash
cut -d',' -f2,3 employees.csv
```

```bash
awk -F',' '$4 > 50000 {print $2, $4}' employees.csv
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
HR
IT
Finance
Sales
```

```bash
sort departments.txt | uniq -c
```

---

## (4) Create `first_names.txt` and `last_names.txt`. Merge them into `full_names.csv` using `paste` with a comma delimiter. Then use `wc -l` to count the number of records.

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

```bash
paste -d',' first_names.txt last_names.txt > full_names.csv
```

```bash
cat full_names.csv
```

```bash
wc -l full_names.csv
```

---

## (5) Create `application.log` containing INFO, WARNING, and ERROR messages. Use `sed` to replace ERROR with CRITICAL and `tr` to convert the final output to uppercase. Display your current working directory.

### Ans:

```bash
nano application.log
```

Example:

```text
INFO: Server Started
WARNING: Low Memory
ERROR: Database Failed
ERROR: Connection Lost
```

Preview replacement:

```bash
sed 's/ERROR/CRITICAL/g' application.log
```

Edit file:

```bash
sed -i 's/ERROR/CRITICAL/g' application.log
```

Convert to uppercase:

```bash
cat application.log | tr 'a-z' 'A-Z'
```

Display current directory:

```bash
pwd
```
