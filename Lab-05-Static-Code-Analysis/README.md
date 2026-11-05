# Lab 5: Static Code Analysis — Car Rental System

**Student Name:** Dharshini V  
**SRN:** PES1UG24AM428  
**Department:** Computer Science & Engineering (AIML), PES University  
**Subject:** Software Engineering Lab (SE Lab) — Lab 5  
**Assigned Source Repository:** `https://github.com/SETAPESU26/L5_56_car-rental`  
**Personal Fork/Repository:** `https://github.com/DharshiniPES/L5_56_car-rental`  

---

## 🎯 Lab Objectives
Use industry-standard static analysis tools (**Pylint**, **Bandit**, and **Flake8**) to inspect, analyze, and repair code quality defects, security vulnerabilities, and PEP 8 style issues in the assigned Python program (`car_rental.py`).

---

## 📈 Tool Analysis Results Summary

| Tool | Focus Area | Before Fixes | After Fixes | Status / Target |
| :--- | :--- | :--- | :--- | :--- |
| **Pylint** | Code Quality, Design & Complexity | **4.94 / 10.00** | **10.00 / 10.00** | ✅ Target > 9.5 exceeded (Perfect score) |
| **Bandit** | Security Vulnerabilities | **11 Issues** (2 High, 4 Medium, 5 Low) | **0 Issues** | ✅ 100% vulnerabilities eliminated |
| **Flake8** | PEP 8 Formatting & Style | **25 Violations** | **0 Violations** | ✅ Fully PEP 8 compliant |

---

## 📁 Deliverables in this Directory

1. **`car_rental.py`**: Cleaned and refactored Python program with all security, code quality, and style defects resolved.
2. **`issues.md`**: Completed issue documentation table detailing 13 distinct findings, lines, CWE/error codes, descriptions, and fix approaches.
3. **`reflection.md`**: In-depth answers to the 4 lab reflection questions discussing tool capabilities, severity prioritization, static analysis limitations, and CI/CD integration.
4. **Before and After Static Analysis Reports**:
   - `pylint_report_before.txt` & `pylint_report_after.txt` (and `pylint_report.txt`)
   - `bandit_report_before.txt` & `bandit_report_after.txt` (and `bandit_report.txt`)
   - `flake8_report_before.txt` & `flake8_report_after.txt` (and `flake8_report.txt`)
