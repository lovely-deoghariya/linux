# Title: Sorting Data with `sort`

---

## (1) Create a file named `fruits.txt` containing 10 fruit names in random order. Display them alphabetically using `sort`.

### Ans:

```bash
nano fruits.txt
```

(Type 10 fruit names, then save and exit.)

```bash
sort fruits.txt
```

---

## (2) Create a file named `numbers.txt` containing the numbers `45`, `2`, `100`, `18`, and `9` on separate lines. Sort them numerically.

### Ans:

```bash
nano numbers.txt
```

(Type the numbers, then save and exit.)

```bash
sort -n numbers.txt
```

---

## (3) Display the fruits in reverse alphabetical order.

### Ans:

```bash
sort -r fruits.txt
```

---

## (4) Create a file named `cities.txt` with duplicate city names. Sort the file and remove duplicate entries.

### Ans:

```bash
nano cities.txt
```

(Type some city names with duplicates, then save and exit.)

```bash
sort -u cities.txt
```

---

## (5) Display your current working directory after completing today's tasks.

### Ans:

```bash
pwd
```
