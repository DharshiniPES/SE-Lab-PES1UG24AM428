# Software Engineering Lab — Individual Submissions

**Student Name:** Dharshini V  
**SRN:** PES1UG24AM428  
**Department:** Department of Computer Science & Engineering (AIML), PES University  
**Course:** Software Engineering Lab (SE Lab)  
**Assigned Project:** Problem Statement #08 — Campus & Academic Operations: **Digital Campus Library Reservation Gateway**  
**Assigned Use Case:** `UC-04: Pay Overdue Fine` (and FR-003: Overdue Fine Calculation & Settlement)  
**Assigned Lab 4 System:** `56_tug_of_war` (Tug of War Game)  
**Assigned Lab 5 System:** `L5_56_car-rental` (Car Rental System)  

---

## 📁 Repository Structure

This repository contains all individual lab submissions for **PES1UG24AM428 (Dharshini V)** with zero external dependencies:

```text
SE-Lab-PES1UG24AM428/
├── .gitignore
├── README.md                                                        # Overview and student metadata
│
├── Lab-01-Requirements-and-UML/                                    # Lab 1: Requirements & Use Cases
│   ├── README.md
│   ├── UC04_Pay_Overdue_Fine_Submission_Dharshini_V_PES1UG24AM428.pdf
│   ├── Requirements_Table.docx
│   ├── Use_Case_Flow_Specification.docx
│   ├── UML_Use_Case_Diagram.png
│   └── UML_Use_Case_Diagram.svg
│
├── Lab-02-Jira-Agile/                                              # Lab 2: Jira Agile & Sprint Execution
│   ├── README.md
│   ├── Jira_Lab2_Final_Submission_Dharshini_V_PES1UG24AM428.pdf
│   └── Jira_Lab2_UC04_Individual_Report_Dharshini_V.docx
│
├── Lab-03-Component-Architecture/                                  # Lab 3: Component Modelling & Architecture
│   ├── README.md
│   ├── Lab3_FINAL_Submission_Dharshini_V_PES1UG24AM428.pdf          # Final report (PDF)
│   ├── Lab3_FINAL_UC04_Dharshini_V_PES1UG24AM428.pdf                # UC-04 specific report (PDF)
│   ├── Lab3_Architecture_Justification_Dharshini_V_PES1UG24AM428.docx # Editable report (Word)
│   ├── Digital_Campus_Library_Component_Diagram.png                # High-resolution diagram (PNG)
│   ├── Digital_Campus_Library_Component_Diagram.svg                # Scalable vector diagram (SVG)
│   ├── Digital_Campus_Library_Component_Diagram.drawio             # Editable Draw.io source
│   └── archive_coffee_kiosk_sample/                                # Archived Coffee Kiosk example assets
│
├── Lab-04-VibeCoding/                                              # Lab 4 (Individual): VibeCoding Tug of War
│   ├── README.md
│   ├── source_code/                                                # Feature-complete Python game
│   ├── videos/                                                     # 10s gameplay verification clips
│   │   ├── TugOfWar_Before.mp4
│   │   └── TugOfWar_After.mp4
│   └── documentation/                                              # Reports & Prompts log
│       ├── Lab4_Final_Submission_Report.pdf
│       ├── Lab4_VibeCoding_Chat_History.pdf
│       └── Lab_4_VibeCoding_Student_handout.pdf
│
└── Lab-05-Static-Code-Analysis/                                    # Lab 5: Pylint, Bandit & Flake8
    ├── README.md
    ├── car_rental.py                                               # Cleaned code (10.00/10, 0 security issues)
    ├── issues.md                                                   # Issue documentation table (13 issues)
    ├── reflection.md                                               # 4 in-depth reflection answers
    ├── pylint_report_before.txt & pylint_report_after.txt          # Pylint reports (4.94 -> 10.00)
    ├── bandit_report_before.txt & bandit_report_after.txt          # Bandit reports (11 issues -> 0)
    └── flake8_report_before.txt & flake8_report_after.txt          # Flake8 reports (25 issues -> 0)
```

---

## 📋 Lab Deliverables Overview

### Lab 1: Requirements Engineering & UML Use-Case Modelling
* **Problem Statement:** #08 — Digital Campus Library Reservation Gateway
* **Assigned Use Case:** `UC-04: Pay Overdue Fine`
* **Deliverables:** PDF report, Requirements Table DOCX, Use-Case Flow Specification DOCX, UML Diagram PNG & SVG.

### Lab 2: Jira Agile — Backlog Creation, Story Point Estimation & Sprint Execution
* **Project:** Digital Campus Library Reservation Gateway
* **Epic:** `EPIC-01: Overdue Fine Payment & Settlement` (21 backlog story points, 13 points completed in Sprint 1)
* **Deliverables:** Final report PDF with Jira screenshots and burndown analysis, editable Word report.

### Lab 3: Component Modelling & Architecture
* **System:** Digital Campus Library Reservation Gateway (`UC-04: Pay Overdue Fine` & FR-003)
* **Architecture:** Layered Architecture (Presentation, Business, Data & External Services layers)
* **Deliverables:** Final report PDF, editable Word report, high-resolution PNG & SVG diagrams, and editable Draw.io model source.

### Lab 4: VibeCoding — Tug of War Game Enhancement
* **VibeCoding Game:** Fixed and enhanced Tug of War Python game (`56_tug_of_war`), before/after screen recordings, prompt engineering chat history, and verification report.

### Lab 5: Static Code Analysis (Pylint, Bandit, Flake8)
* **Assigned Script:** Car Rental System (`car_rental.py` from `SETAPESU26/L5_56_car-rental`)
* **Personal Repository:** `https://github.com/DharshiniPES/L5_56_car-rental` (3 distinct commits for Bandit, Pylint, and Flake8 fixes)
* **Results Achieved:**
  * **Pylint Score:** Improved from **4.94 / 10.00** to **10.00 / 10.00** (exceeding > 9.5 target)
  * **Bandit:** Eliminated all **11 security vulnerabilities** (0 High, 0 Medium, 0 Low)
  * **Flake8:** Resolved all **25 PEP 8 formatting/style violations** (0 remaining)
* **Deliverables:** Cleaned `car_rental.py`, comprehensive `issues.md` remediation table, detailed `reflection.md` report, and before/after verification logs.
