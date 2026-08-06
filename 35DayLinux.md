# Title: Combining Files with `paste`

---

## (1) Create `names.txt` and `departments.txt` with five matching lines. Combine them using `paste`.

### Ans:

```bash
nano names.txt
```

(Type names, save and exit.)

```bash
nano departments.txt
```

(Type departments, save and exit.)

```bash
paste names.txt departments.txt
```

---

## (2) Combine `names.txt` and `departments.txt` using a comma as the delimiter.

### Ans:

```bash
paste -d ',' names.txt departments.txt
```

---

## (3) Create `ids.txt` and combine `ids.txt`, `names.txt`, and `departments.txt` into one output.

### Ans:

```bash
nano ids.txt
```

(Type IDs, save and exit.)

```bash
paste ids.txt names.txt departments.txt
```

---

## (4) Save the combined output into `employees.csv` and display it using `cat`.

### Ans:

```bash
paste -d ',' ids.txt names.txt departments.txt > employees.csv
cat employees.csv
```

---

## (5) Display your current working directory after completing today's tasks.

### Ans:

```bash
pwd
```
