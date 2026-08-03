# Title: Removing Duplicate Lines with `uniq`

---

## (1) Create a file named `names.txt` with duplicate names. Sort it and remove duplicate lines.

### Ans:

```bash
nano names.txt
```

(Type some duplicate names, then save and exit.)

```bash
sort names.txt | uniq
```

---

## (2) Count how many times each name appears using `uniq -c`.

### Ans:

```bash
sort names.txt | uniq -c
```

---

## (3) Display only duplicate names using `uniq -d`.

### Ans:

```bash
sort names.txt | uniq -d
```

---

## (4) Display only names that appear exactly once using `uniq -u`.

### Ans:

```bash
sort names.txt | uniq -u
```

---

## (5) Display your current working directory after completing today's tasks.

### Ans:

```bash
pwd
```
