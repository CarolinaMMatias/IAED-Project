# Vaccine Management System — C

Project developed for the **Introdução aos Algoritmos e Estruturas de Dados** (Introduction to Algorithms and Data Structures) course at **Instituto Superior Técnico (IST)**.

---

## 💉 About the Project

A command-line system written in **C** to manage vaccine batches, stock, expiration dates, user inoculations, and simulated time.

---

## ⚙️ Core Commands

* **`c`**: Adds a new vaccine batch (batch ID, expiration date, number of doses, vaccine name).
* **`l`**: Lists available batches ordered by expiration date and batch ID.
* **`a`**: Inoculates a user with the oldest valid available batch (prevents duplicate doses on the same day).
* **`r`**: Removes or cancels remaining doses of a specific batch.
* **`d`**: Deletes inoculation records (by user, date, or batch).
* **`u`**: Lists inoculation history chronologically (all or filtered by user).
* **`t`**: Displays or advances the simulated system calendar.
* **`q`**: Cleans up all dynamic memory and exits the program.

---

## 🛠️ Implementation & Constraints

* **Language**: C
* **Memory Management**: Fully dynamic allocation (`malloc`/`free`) with zero memory leaks (verified using `valgrind`).
* **Clean Code**: No global variables, no `goto`, and custom sorting algorithms (native `qsort` not allowed).
* **Bilingual Support**: Standard English output or Portuguese error messages when run with `./proj pt`.

---

## 💻 Compilation & Execution

Compile using `gcc` with strict flags:

```bash
gcc -O3 -Wall -Wextra -Werror -Wno-unused-result -o proj *.c
