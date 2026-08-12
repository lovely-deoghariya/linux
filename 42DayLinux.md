# Title: Compressing Files with gzip and gunzip

---

## (1) Create a file named `report.txt` and compress it using gzip.

### Ans:

```bash
nano report.txt
```

Example:

```text
This is a sample report file.
Linux compression practice.
```

```bash
gzip report.txt
```

---

## (2) Decompress `report.txt.gz` using gunzip and verify the original file is restored.

### Ans:

```bash
gunzip report.txt.gz
```

```bash
ls
```

---

## (3) Create another file named `logs.txt` and compress it while keeping the original file.

### Ans:

```bash
nano logs.txt
```

Example:

```text
INFO: Server Started
WARNING: Low Memory
ERROR: Connection Failed
```

```bash
gzip -k logs.txt
```

```bash
ls
```

---

## (4) Create a folder named `demo_project` containing two files. Create a compressed archive named `demo_project.tar.gz` using tar and gzip together.

### Ans:

```bash
mkdir demo_project

touch demo_project/file1.txt
touch demo_project/file2.txt

tar -czvf demo_project.tar.gz demo_project/
```

---

## (5) Display your current working directory and list all `.gz` files.

### Ans:

```bash
pwd
```

```bash
ls *.gz
```

---

## Mini Challenge

### Ans:

```bash
mkdir data_backup

touch data_backup/employees.csv
touch data_backup/sales.csv
touch data_backup/application.log

tar -czvf data_backup.tar.gz data_backup/

tar -tzvf data_backup.tar.gz

mkdir restore_backup

tar -xzvf data_backup.tar.gz -C restore_backup/

ls -R restore_backup/

pwd
```
