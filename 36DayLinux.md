# Title: Transforming Text with `tr`

---

## (1) Create a file named `names.txt` with lowercase names. Convert them to uppercase using `tr`.

### Ans:

```bash
nano names.txt
```

(Type lowercase names, save and exit.)

```bash
cat names.txt | tr 'a-z' 'A-Z'
```

---

## (2) Create a file with uppercase text and convert it to lowercase.

### Ans:

```bash
nano upper.txt
```

(Type uppercase text, save and exit.)

```bash
cat upper.txt | tr 'A-Z' 'a-z'
```

---

## (3) Create a file containing commas and remove all commas using `tr -d`.

### Ans:

```bash
nano data.txt
```

(Type text with commas, save and exit.)

```bash
cat data.txt | tr -d ','
```

---

## (4) Create a file with multiple consecutive spaces. Use `tr -s` to squeeze repeated spaces into a single space.

### Ans:

```bash
nano text.txt
```

(Type text with multiple spaces, save and exit.)

```bash
cat text.txt | tr -s ' '
```

---

## (5) Display your current working directory after completing today's tasks.

### Ans:

```bash
pwd
```
