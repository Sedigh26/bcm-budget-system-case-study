# Case Study: BCM-AEMS (Sovereign Budget Execution System)

## 🏦 Project Overview
The **BCM-AEMS** is a high-security enterprise application developed for the **Banque Centrale de Mauritanie (BCM)**. The system was designed to transform manual, Excel-based budgetary tracking into a centralized, secure, and auditable digital ecosystem.

> **Note:** To maintain the security and confidentiality of a national financial institution, the source code is private. This repository serves as a technical documentation of the architecture and engineering decisions.

---

## 🛠️ Technical Stack (Modern Monolith)
I implemented a **Three-Tier Architecture** to ensure a strict separation of concerns and high security:

- **Frontend (Presentation Layer):** `React 18` & `Tailwind CSS`. Developed as a Single Page Application (SPA) for a fluid user experience.
- **Backend (Business Layer):** `Laravel 11 (PHP 8.2)`. Utilized the **Action-Service Pattern** to isolate financial logic for better auditability.
- **The Bridge:** `Inertia.js`. Used to connect Laravel and React, allowing for server-side routing with a client-side reactive UI.
- **Database (Data Layer):** `MySQL 8`. Guaranteed **ACID compliance** to ensure that no financial transaction is partially recorded or lost.

---

## 🔒 Enterprise-Grade Security & Logic
This project required strict banking standards. I implemented the following professional protocols:

### 1. The Maker-Checker Principle (Four-Eyes Principle)
To prevent fraud and errors, the system enforces a dual-authorization workflow:
- **Maker (Finance/Staff):** Initiates the transaction (Status: `Pending`).
- **Checker (Administrator):** Reviews and provides the final sovereign validation (`Approved` or `Rejected`).

### 2. Advanced Security Layer
- **Cryptographic Validation:** Implemented `Bcrypt` hashing (Rounds=12) for passwords.
- **Session Security:** Implemented **Session ID Regeneration** after login to prevent *Session Fixation* attacks.
- **Access Control:** Strict **RBAC (Role-Based Access Control)** to ensure data silos between different institutional roles.
- **Audit Trail:** A dedicated `Activity Log` system that records every single action (Login, Update, Export) for full traceability.

---

## 📊 Key Engineering Features
- **Analytical Dashboard:** Built with `Recharts` to provide real-time visual monitoring of budget consumption.
- **Budgetary Logic:** A custom engine that calculates balances and triggers "Chromatic Alerts" (Green/Amber/Red) when budget thresholds are reached.
- **Institutional Export:** Automated generation of secure `PDF` and `Excel (XLSX)` reports for official auditing.

---

## 📈 Impact
- **Digitization:** Replaced fragmented Excel files with a "Single Source of Truth."
- **Risk Reduction:** Eliminated manual entry errors and provided an immutable audit trail.
- **Efficiency:** Reduced the time for budget reporting and executive decision-making through real-time analytics.

## 🧠 Lessons Learned
- Mastering the **Modern Monolith** stack (Laravel + Inertia + React).
- Designing for **Financial Integrity** (ACID, Maker-Checker).
- Building for **Sovereign Institutions** where security is more important than speed.
