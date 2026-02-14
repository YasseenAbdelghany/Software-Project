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

### Core Documentation
- [BinWise documentation Final.pdf](BinWise%20documentation%20Final.pdf) — Complete system documentation
- [Design Report.pdf](Design%20Report.pdf) — Detailed design specifications
- [RVM Report.pdf](RVM%20Report.pdf) — Main project report
- [TestReport.pdf](TestReport.pdf) — Testing and validation plan

### Proposals & Research
- [RVM-Proposal.pdf](RVM-Proposal.pdf) — Initial project proposal
- [RVM_Research_Paper.pdf](RVM_Research_Paper.pdf) — Research findings

### Architecture & Design Diagrams
- [Context Diagram(Level0).png](Context%20Diagram(Level0).png) — System context diagram
- [Level1-Architecture.pdf](Level1-Architecture.pdf) — Level 1 architecture
- [ArchLevel 3.pdf](ArchLevel%203.pdf) — Level 3 detailed architecture
- [UseCase Diagram.png](UseCase%20Diagram.png) — Use case diagram
- [SEQUANCE-Diagrams.zip](SEQUANCE-Diagrams.zip) — Sequence diagrams (zipped)

### Use Case & Estimation
- [RVM System — Use Case Estimation .pdf](RVM%20System%20%E2%80%94%20Use%20Case%20Estimation%20.pdf) — Use case estimation

### Survey & Presentations
- [RVM_Survey_Report.pdf](RVM_Survey_Report.pdf) — User survey analysis
- [RVM_Survey_Presentation.pptx](RVM_Survey_Presentation.pptx) — Survey presentation
- [Recyle vending Designs.pptx](Recyle%20vending%20Designs.pptx) — Design presentation

### Ethics
- [Ethics Report-Smart Reverse Vending Machine.pdf](Ethics%20Report-Smart%20Reverse%20Vending%20Machine.pdf) — Ethics considerations

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