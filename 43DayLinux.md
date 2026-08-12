# Title: Creating and Extracting ZIP Archives

---

## (1) Create a folder named `project_files` containing `README.md`, `employees.csv`, and `notes.txt`. Compress it into `project_files.zip`.

### Ans:

mkdir project_files

touch project_files/README.md
touch project_files/employees.csv
touch project_files/notes.txt

zip -r project_files.zip project_files/

---

## (2) List the contents of `project_files.zip` without extracting it.

### Ans:

unzip -l project_files.zip

---

## (3) Extract `project_files.zip` into a folder named `extracted_project`.

### Ans:

mkdir extracted_project

unzip project_files.zip -d extracted_project

---

## (4) Create a file named `changelog.txt` and add it to the existing ZIP archive using the update option.

### Ans:

touch changelog.txt

zip -u project_files.zip changelog.txt

---

## (5) Display your current working directory and list all ZIP files.

### Ans:

pwd

ls *.zip
