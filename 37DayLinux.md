# Title: Editing Text with `sed`

---

## (1) Create `fruits.txt` with several occurrences of the word Apple. Replace the first Apple on each line with Mango using sed.

### Ans:

```bash
nano fruits.txt
```

Example content:

```text
Apple Apple Banana
Apple Orange Apple
Apple Grapes
```

```bash
sed 's/Apple/Mango/' fruits.txt
```

---

## (2) Replace every occurrence of Apple with Mango using the global option.

### Ans:

```bash
sed 's/Apple/Mango/g' fruits.txt
```

---

## (3) Create `employees.txt` with at least 10 lines. Display only lines 1 to 5 using sed.

### Ans:

```bash
nano employees.txt
```

(Add at least 10 lines, save and exit.)

```bash
sed -n '1,5p' employees.txt
```

---

## (4) Create `config.txt` containing the word development several times. Replace development with production directly in the file using `sed -i`, then verify the changes with `cat`.

### Ans:

```bash
nano config.txt
```

Example content:

```text
development
development server
development mode
```

```bash
sed -i 's/development/production/g' config.txt
```

```bash
cat config.txt
```

---

## (5) Display your current working directory after completing today's tasks.

### Ans:

```bash
pwd
```
