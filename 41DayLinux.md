# Title: Creating and Extracting Archives with tar

---

## (1) Create a folder named `project_backup` containing `README.md`, `employees.csv`, and `application.log`. Create a TAR archive named `project_backup.tar`.

### Ans:

```bash
mkdir project_backup

touch project_backup/README.md
touch project_backup/employees.csv
touch project_backup/application.log

tar -cvf project_backup.tar project_backup/
```

---

## (2) List the contents of `project_backup.tar` without extracting it.

### Ans:

```bash
tar -tvf project_backup.tar
```

---

## (3) Create a folder named `restore` and extract `project_backup.tar` into it.

### Ans:

```bash
mkdir restore

tar -xvf project_backup.tar -C restore/
```

---

## (4) Verify that all extracted files exist using `ls`.

### Ans:

```bash
ls restore/project_backup/
```

---

## (5) Display your current working directory after completing today's tasks.

### Ans:

```bash
pwd
```

---

## Mini Challenge

### Ans:

```bash
mkdir -p data_pipeline/data
mkdir -p data_pipeline/logs
mkdir -p data_pipeline/scripts

touch data_pipeline/data/employees.csv
touch data_pipeline/logs/app.log
touch data_pipeline/scripts/process.sh

tar -cvf data_pipeline.tar data_pipeline/

tar -tvf data_pipeline.tar

mkdir extracted_data

tar -xvf data_pipeline.tar -C extracted_data/

ls -R extracted_data/

pwd
```
