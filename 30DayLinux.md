# Title: Common Linux Permission Values (644, 755, 600, 700)

---

## (1) Create a file named `notes.txt` and set its permissions to `644`. Verify using `ls -l`.

### Ans:

```bash
touch notes.txt
chmod 644 notes.txt
ls -l notes.txt
```

---

## (2) Create a shell script named `pipeline.sh` and set its permissions to `755`.

### Ans:

```bash
touch pipeline.sh
chmod 755 pipeline.sh
ls -l pipeline.sh
```

---

## (3) Create a file named `secrets.txt` and set its permissions to `600`.

### Ans:

```bash
touch secrets.txt
chmod 600 secrets.txt
ls -l secrets.txt
```

---

## (4) Create a directory named `private_data` and set its permissions to `700`. Verify the result.

### Ans:

```bash
mkdir private_data
chmod 700 private_data
ls -ld private_data
```

---

## (5) Display your current working directory and list all files with detailed permissions.

### Ans:

```bash
pwd
ls -l
```
