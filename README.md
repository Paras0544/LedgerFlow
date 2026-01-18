# LedgerFlow: Enterprise Retail Banking Portal 🏦

> **Development Status:** This project is under active development. Core MERN-stack modules for secure fund transfers and audit logging are currently being integrated. 🏗️

## 📌 Project Overview
LedgerFlow is a high-integrity, full-stack retail banking dashboard designed to simulate the complexities of enterprise-grade financial systems. The application prioritizes **data consistency**, **secure session management**, and **auditability** to ensure a world-class digital banking experience.

## 🛠 Technical Stack
* **Frontend:** React.js, Redux Toolkit (State Management), Tailwind CSS
* **Backend:** Node.js, Express.js
* **Database:** MongoDB (Atlas)
* **Security:** JWT (JSON Web Tokens), Bcrypt.js for password hashing
* **Operations:** RESTful API architecture, Git version control

## 🏗 Key Engineering Features
* **ACID-Compliant Transactions:** Implemented Mongoose sessions to handle fund transfers. This ensures that a transaction either completes fully or rolls back entirely, preventing data corruption or "phantom" balances.
* **Secure-by-Design Auth:** Integrated JWT-based authentication with protected API routes. The system is designed to prevent common vulnerabilities like unauthorized access and session hijacking.
* **Audit Logging System:** Built a backend logging module that records every sensitive action (login, logout, fund transfer). This mirrors the "Probity" and "Compliance" requirements standard in global banking (GCC).
* **Performance Optimization:** Utilized Redux for global state management to ensure seamless UI updates across the dashboard without unnecessary database polling.



## 🚀 Challenges & Solutions
* **The Race Condition Challenge:** Identified a risk where concurrent withdrawal requests could exceed the actual balance. Resolved this by implementing atomic database updates and strict server-side validation logic.
* **Scalability:** Designed the backend using a modular controller-service pattern, making it easier to add new retail products like "Fixed Deposits" or "Forex Tracking" in the future.

## 🛠 Setup & Installation
1.  **Clone:** `git clone https://github.com/Paras0544/LedgerFlow.git`
2.  **Dependencies:** Run `npm install` in both the root and client folders.
3.  **Environment:** Configure a `.env` file with your `MONGO_URI` and `JWT_SECRET`.
4.  **Launch:** Execute `npm run dev` to start the development server.

---
**Developed by: Paras Miglani**
