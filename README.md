# Smart Reverse Vending Machine (RVM) — Design Project

A **system design + software architecture** project for a Smart Reverse Vending Machine (RVM) that encourages campus plastic recycling through **QR-based identification**, **gamification**, and **rewards**.

Students scan a personal QR code, deposit recyclables, and earn points based on weight. The proposed system includes **Raspberry Pi–based RVM hardware** (with sensors for validation), a **mobile app** for students, and an **admin web dashboard** for monitoring and management.

> Note: This repository contains **design documentation** (requirements, diagrams, reports, and test plan). It is not a complete runnable implementation.

---

## What the system aims to do

- Reduce campus plastic waste by making recycling **engaging and measurable**.
- Prevent recycling-stream contamination via **material classification** and **liquid detection**.
- Provide a campus-wide incentive loop: points can be redeemed (e.g., at the cafeteria) and tracked via leaderboards.

---

## Key features (designed)

- **QR-based user identification** (students) + **Guest mode** (for visitors/staff without registration)
- **Points system** based on deposited weight (transparent calculation)
- **Leaderboards** (student vs. student, college vs. college)
- **Rewards redemption** flow
- **AI-assisted material classification** (plastic vs. non-plastic) with diversion to prevent contamination
- **Liquid detection** to reject bottles with liquid and protect recycling quality
- **Offline-first RVM operation** with automatic sync when connectivity returns
- **Admin monitoring**: capacity alerts (e.g., at 80%), machine health/sensor malfunction notifications, analytics & reports

---

## High-level architecture (designed)

- **RVM Device (IoT)**
  - Raspberry Pi
  - QR scanner / camera module
  - Weight sensor (load cell)
  - Liquid detection sensors (weight/tilt approach)
  - Material classification component (AI-based)

- **Software system**
  - **Student mobile app**: QR code access, points balance, transaction history, leaderboards, reward redemption
  - **Admin web dashboard**: machine monitoring, inventory/rewards management, analytics, reports, multi-machine management
  - **Backend + database (designed)**: user accounts, transactions, points ledger, notifications, machine alerts, QR lifecycle

---

## Documentation in this repo

These files describe the project requirements, architecture, diagrams, and validation plan:

- [Design Report.pdf](Design%20Report.pdf)
- [RVMProposal.pdf](RVMProposal.pdf)
- [TestReport.pdf](TestReport.pdf)
- [Level1 arc finall.pdf](Level1%20arc%20finall.pdf)
- [ClasssDiagram.excalidrawadel final.pdf](ClasssDiagram.excalidrawadel%20final.pdf)
- [Recyle vending machine.pptx](Recyle%20vending%20machine.pptx)
- [RVM_Survey_Report.pdf](RVM_Survey_Report.pdf)
- [RVM_Survey_Presentation.pptx](RVM_Survey_Presentation.pptx)
- [ahm-ethicfinal321.pdf](ahm-ethicfinal321.pdf)

Optional (generated for easier searching in VS Code):
- [docs_extracted/ALL_EXTRACTED_TEXT.md](docs_extracted/ALL_EXTRACTED_TEXT.md)

---

## Project scope

This project focuses on **system design**:
- Functional requirements (e.g., QR scan/validation, item validation, points, rewards, leaderboards)
- Architecture and subsystem design (SOLID-oriented design approach)
- Database design (entities for users, machines, transactions, points ledger, alerts, etc.)
- Test plan / test cases (validation approach)

---

## Team

- Yasseen Ahmed El-Sayed
- Mohamed Mustafa Awad
- Ahmed Khaled Said
- Marawan Khaled Ahmed
- Mohamed Adel Abdulrahman
