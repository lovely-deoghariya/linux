# Title: Viewing Running Processes with ps

---

## (1) Run the ps command and observe the processes attached to your current terminal.

### Ans:

ps

---

## (2) Run ps -e and count how many processes are displayed.

### Ans:

ps -e

ps -e | wc -l

---

## (3) Run ps -ef and identify the PID of your shell (bash or zsh if shown).

### Ans:

ps -ef

ps -ef | grep bash

---

## (4) Run ps aux and locate the process running your current shell.

### Ans:

ps aux

ps aux | grep bash

---

## (5) Display your current working directory after completing today's tasks.

### Ans:

pwd
