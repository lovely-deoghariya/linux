# Title: Changing Permissions with `chmod`

---

## (1) Create a file named `script.sh` and view its permissions using `ls -l`.

### Ans:

```bash
touch script.sh
ls -l script.sh
```

---

## (2) Give the owner execute permission on `script.sh` using symbolic mode, then verify the change.

### Ans:

```bash
chmod u+x script.sh
ls -l script.sh
```

---

## (3) Create a file named `report.txt` and remove write permission from the group.

### Ans:

```bash
touch report.txt
chmod g-w report.txt
ls -l report.txt
```

---

## (4) Change the permissions of `report.txt` to `644` using numeric mode and verify with `ls -l`.

### Ans:

```bash
chmod 644 report.txt
ls -l report.txt
```

---

## (5) Display your current working directory after completing today's tasks.

### Ans:

```bash
pwd
```
