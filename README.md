# bcm-budget-system-case-study
A technical case study of a sovereign budget management system designed for the Direction Générale of BCM.
# Case Study: Sovereign Budget Management System (BCM-AEMS)

## 📌 Project Overview
The **BCM-AEMS** is a high-security, enterprise-level budget management system developed for the **Direction Générale of BCM**. The primary goal was to digitize the sovereign budgetary process, replacing manual tracking with a secure, automated, and transparent digital workflow.

> **Note:** Due to the sensitive nature of the project and institutional privacy agreements, the source code is hosted in a private repository. This repository serves as a technical case study of the architecture and implementation.

---

## 🚀 The Challenge
The institution faced several critical challenges:
- **Data Fragmentation:** Budgetary data was spread across multiple spreadsheets and physical documents.
- **Lack of Real-time Tracking:** No centralized way to monitor spending versus allocation in real-time.
- **Security Risks:** Need for strict Role-Based Access Control (RBAC) to ensure only authorized personnel could approve financial movements.

## 🛠️ Technical Solution

### 1. System Architecture
I implemented a **Full-Stack Architecture** designed for stability and data integrity:
- **Frontend:** Developed a responsive administrative dashboard focusing on data visualization (charts, tables, and reports) for executive decision-making.
- **Backend:** Built a robust API layer to handle complex financial calculations and ensure atomic transactions (ensuring no budget is "lost" during updates).
- **Database:** Designed a relational schema optimized for financial auditing, ensuring every change is logged with a timestamp and user ID.

### 2. Key Features Implemented
- **Automated Budget Allocation:** Logic to distribute funds across departments based on predefined rules.
- **Approval Workflow:** A multi-step verification system where requests move from "Pending" $\rightarrow$ "Reviewed" $\rightarrow$ "Approved."
- **Financial Reporting:** Automated generation of budget vs. actual spending reports.
- **RBAC Security:** Custom middleware to manage permissions for different administrative levels.

### 3. Tech Stack Used
- **Languages:** `JavaScript`, `SQL`
- **Frontend:** `React.js` / `Tailwind CSS` (or specify your framework)
- **Backend:** `Node.js` / `PHP` (or specify your framework)
- **Database:** `MySQL` / `PostgreSQL`

---

## 📈 Impact & Results
- **Efficiency:** Reduced the time required for budget reporting by [X]% (e.g., 50%).
- **Accuracy:** Eliminated human error in budget calculations through automated validation.
- **Transparency:** Provided the Direction Générale with a "Single Source of Truth" for all financial data.

## 🧠 Engineering Lessons Learned
- **Handling Sensitive Data:** Learned how to implement strict data validation to prevent financial discrepancies.
- **User-Centric Design:** Learned how to build interfaces for non-technical administrative staff.
- **Scalability:** Designed the database to handle increasing amounts of financial records over several fiscal years.
