# Title: Practical Assignment - Compression & Archiving

---

## (1) Create a folder named data_pipeline containing data/, logs/, and scripts/ subfolders. Add employees.csv, sales.csv, application.log, and run.sh with sample content.

### Ans:

mkdir -p data_pipeline/data
mkdir -p data_pipeline/logs
mkdir -p data_pipeline/scripts

touch data_pipeline/data/employees.csv
touch data_pipeline/data/sales.csv
touch data_pipeline/logs/application.log
touch data_pipeline/scripts/run.sh

---

## (2) Create a TAR archive named data_pipeline.tar. List its contents without extracting it.

### Ans:

tar -cvf data_pipeline.tar data_pipeline/

tar -tvf data_pipeline.tar

---

## (3) Create a compressed archive named data_pipeline.tar.gz. Extract it into a folder named restore_tar and verify the restored files.

### Ans:

tar -czvf data_pipeline.tar.gz data_pipeline/

mkdir restore_tar

tar -xzvf data_pipeline.tar.gz -C restore_tar

ls restore_tar

---

## (4) Create a ZIP archive named data_pipeline.zip. List its contents, then extract it into a folder named restore_zip.

### Ans:

zip -r data_pipeline.zip data_pipeline/

unzip -l data_pipeline.zip

mkdir restore_zip

unzip data_pipeline.zip -d restore_zip

---

## (5) Compress application.log using gzip while keeping the original file. Verify the .gz file exists, then display your current working directory.

### Ans:

gzip -k data_pipeline/logs/application.log

ls data_pipeline/logs/

pwd
