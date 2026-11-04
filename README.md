# Software Engineering Lab — Individual Submissions

**Student Name:** Dharshini V  
**SRN:** PES1UG24AM428  
**Department:** Department of Computer Science & Engineering (AIML), PES University  
**Course:** Software Engineering Lab (SE Lab)  
**Assigned Project:** Problem Statement #08 — Campus & Academic Operations: **Digital Campus Library Reservation Gateway**  
**Assigned Use Case:** `UC-04: Pay Overdue Fine` (and FR-003: Overdue Fine Calculation & Settlement)

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
│       ├── 480.drawio
│       ├── Lab3_Coffee_Kiosk_Component_Diagram.drawio
│       ├── Lab3_Coffee_Kiosk_Component_Diagram_FIXED.png
│       ├── Lab3_Coffee_Kiosk_Justification.docx
│       └── Lab3_Coffee_Kiosk_Original_Submission.pdf
│
├── Lab-04-SRS-SAD-STP/                                             # Lab 4 (Milestone): SRS, SAD & Test Plan
│   ├── README.md
│   ├── SRS_Library_Reservation_Gateway (1).pdf                     # Software Requirements Specification
│   ├── SAD_Library_Reservation_Gateway (1).pdf                     # Software Architecture & Design
│   └── Test_Plan_Library_Reservation_Gateway.docx                  # Software Test Plan
│
└── Lab-04-VibeCoding/                                              # Lab 4 (Individual): VibeCoding Tug of War
    ├── README.md
    ├── source_code/                                                # Feature-complete Python game
    │   ├── main.py
    │   ├── README.md
    │   └── game/
    │       ├── game_engine.py
    │       ├── player.py
    │       └── rope.py
    ├── videos/                                                     # 10s gameplay verification clips
    │   ├── TugOfWar_Before.mp4
    │   └── TugOfWar_After.mp4
    └── documentation/                                              # Reports & Prompts log
        ├── Lab4_Final_Submission_Report.pdf
        ├── Lab4_VibeCoding_Chat_History.pdf
        └── Lab_4_VibeCoding_Student_handout.pdf
```

---

## 📋 Lab Deliverables Overview

### Lab 1: Requirements Engineering & UML Use-Case Modelling
* **Problem Statement:** #08 — Digital Campus Library Reservation Gateway
* **Assigned Use Case:** `UC-04: Pay Overdue Fine`
* **Actors:** Primary: Student Member | Supporting: Payment Gateway (external), Head Librarian (`«extend»` UC-06 Apply Fine Waiver)
* **Key Deliverables:**
  * `UC04_Pay_Overdue_Fine_Submission_Dharshini_V_PES1UG24AM428.pdf`: Complete compiled report.
  * `Requirements_Table.docx`: Functional requirements (FR-001 to FR-005) and non-functional requirements (NFR-001 latency < 150ms, NFR-002 99.5% uptime).
  * `Use_Case_Flow_Specification.docx`: Preconditions, postconditions, main success flow (8 steps), and alternate flow 5a (payment declined).
  * `UML_Use_Case_Diagram.png` & `.svg`: Exported UML Use Case diagram.

### Lab 2: Jira Agile — Backlog Creation, Story Point Estimation & Sprint Execution
* **Project:** Digital Campus Library Reservation Gateway
* **Epic:** `EPIC-01: Overdue Fine Payment & Settlement`
* **Backlog:** 6 User Stories (`DCLRG-2` to `DCLRG-7`), 21 total story points.
* **Sprint 1 Execution:** 4 stories planned (`DCLRG-2`, `DCLRG-3`, `DCLRG-4`, `DCLRG-5`), 13 story points burned down to 0 on the Scrum board.
* **Key Deliverables:**
  * `Jira_Lab2_Final_Submission_Dharshini_V_PES1UG24AM428.pdf`: Comprehensive submission document with story point estimates, Jira epic screenshots, sprint execution board, and burndown chart analysis.
  * `Jira_Lab2_UC04_Individual_Report_Dharshini_V.docx`: Editable Word report.

### Lab 3: Component Modelling & Architecture (Updated)
* **Assigned System:** Digital Campus Library Reservation Gateway (Problem Statement #08)
* **Subsystem Focus:** Fine Management & Payment Settlement (`UC-04: Pay Overdue Fine` & FR-003)
* **Selected Architectural Style:** **Layered Architecture**
  * **Presentation Layer:** Student Member UI Component (Balance lookup, itemized fines, payment selection)
  * **Business Layer:**
    * *Authentication & Session Component* (Credential validation, SSO, role enforcement)
    * *Fine Management Component (UC-04)* (Calculates ₹5/day overdue capped at ₹200, handles settlement, triggers receipts)
    * *Notification Service Component* (Dispatches payment confirmation and itemized receipts via email)
  * **Data & External Services Layer:**
    * *Payment Gateway Adapter* (Interfaces Credit/Debit Card, UPI, and Campus Wallet)
    * *Library Database Component* (Persists student fine balances, transaction logs, hold queue)
    * *External Campus SMTP Server* (Campus mail relay)
* **Interfaces (Ball & Socket):** `IAuthentication`, `IFineService`, `IPaymentGateway`, `IFineData/SQL`, `INotification`, `ISMTPRelay`.
* **Key Deliverables:**
  * `Lab3_FINAL_Submission_Dharshini_V_PES1UG24AM428.pdf` & `Lab3_FINAL_UC04_Dharshini_V_PES1UG24AM428.pdf`: Compiled final submission PDFs.
  * `Lab3_Architecture_Justification_Dharshini_V_PES1UG24AM428.docx`: Editable Word justification document.
  * `Digital_Campus_Library_Component_Diagram.png` & `.svg`: High-resolution component diagram exports.
  * `Digital_Campus_Library_Component_Diagram.drawio`: Editable Draw.io source.

### Lab 4: Project Specifications & VibeCoding
1. **SRS, SAD & Test Plan:**
   * **SRS:** Complete functional and non-functional requirements specification for Digital Campus Library Reservation Gateway.
   * **SAD:** Detailed architecture, layered component design, interface contracts, and sequence interactions.
   * **STP:** Comprehensive test cases and validation matrices for fine calculation, payment gateway hooks, and hold queues.
2. **VibeCoding Tug of War:**
   * **Source Code:** Debugged and enhanced Python game (`main.py`, `game/` engine, rope dynamics, player controls).
   * **Features:** Key input debounce, AI panic surge, rope tension animations, 45-second match timer, and Sudden Death mode.
   * **Recordings:** Screen recordings before and after feature implementation.
   * **Documentation:** Prompt work log and final test verification report.
