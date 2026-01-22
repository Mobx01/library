# Library Book Management System  
### Agile Development with Git and Unit Testing (CS2042 – SWE Task 1)

##  Overview

This project is a **Library Book Management System** developed in **Python** as part of a Software Engineering assignment.  
The primary goal of this project is to demonstrate **Agile sprint-based development**, **Git workflow discipline**, **unit testing**, and **traceability**, rather than building a large production system.

The system operates entirely using **in-memory data structures** (no database).

---

##  Features

- Add books with Book ID, Title, and Author
- Prevent duplicate Book IDs
- Borrow and return books
- Prevent borrowing of unavailable books
- Generate a library status report
- Fully tested using Python `unittest`
- Developed using 3 Agile sprints with Git branches and tags

---

##  Technologies Used

- Programming Language: **Python 3**
- Testing Framework: **unittest**
- Version Control: **Git & GitHub**

---


---

##  How to Run This Project on Your Computer

### 1️ Prerequisites

Ensure the following are installed:

- Python 3  
python --version

- Git  
git --version

---

### 2️ Clone the Repository

git clone <repository-url>
cd library

---

### 3️ Run Unit Tests (Recommended)

This project does not include a graphical interface.  
All functionality is validated through **unit tests**.

Run all tests using:
python -m unittest discover -s tests -p "test_*.py" -v

If all tests pass, the system is working correctly.

---

## How the System Works

### Add Book
- A book is added with a unique Book ID, title, and author.
- Attempting to add a duplicate Book ID raises an error.

### Borrow Book
- A book can be borrowed only if it is available.
- Borrowing an already borrowed book raises an error.

### Return Book
- Returning a book updates its availability status.

### Generate Report
- Generates a report containing:
  - Book ID
  - Title
  - Author
  - Status (Available / Borrowed)

---

##  Agile Development & Git Workflow

This project was implemented using **three Agile sprints**.

| Sprint | Feature Implemented | Git Tag |
|------|--------------------|--------|
| Sprint 1 | Book Registration | v0.1 |
| Sprint 2 | Borrow & Return | v0.2 |
| Sprint 3 | Library Report | v0.3 |

### Git Practices Followed

- Each sprint was developed in a separate branch:
  - `feature/sprint-1`
  - `feature/sprint-2`
  - `feature/sprint-3`
- Sprint branches were merged into the `main` branch
- Each sprint release was marked with a Git tag

---

##  Useful Git Verification Commands

git branch -r
git tag
git log --all --oneline --decorate --graph
---

## 📖 Documentation

- `docs/USER_STORIES.md`  
  Contains sprint-wise user stories.

- `docs/TRACEABILITY.md`  
  Maps user stories to implemented features, unit tests, and Git tags.

---

##  Key Learnings

- Agile sprint planning and execution
- Git branching, merging, and tagging discipline
- Writing unit tests for verification
- Maintaining traceability from requirements to implementation and release

---

##  License

This project was developed for academic purposes as part of a university assignment.





