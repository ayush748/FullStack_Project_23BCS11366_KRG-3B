# ☁️ Cloud Share — Full Stack Secure File Sharing SaaS

## 📘 1. Introduction

**Cloud Share** is a modern full-stack web application built for **secure file upload, storage, and sharing**.  
It demonstrates enterprise-grade architecture and uses the following stack:

- **Frontend:** React.js + Tailwind CSS  
- **Backend:** Spring Boot (Java)  
- **Database:** MongoDB  
- **Authentication:** Clerk  
- **Payments:** Razorpay  

> 🏗️ The goal: Build a scalable, secure SaaS file-sharing platform with real-world integrations.

---

## 🧩 2. Problem Identification



In modern development, applications must securely manage:
1. **User Identity & Access Control**
2. **File Integrity & Security**
3. **Payment & Transactional Reliability**

**Cloud Share** solves these with enterprise-grade authentication, backend validation, and transactional safety.

---

## 📚 3. Literature Review / Background Study

### 3.1 Existing Solutions
- Many existing systems are either **too simple (no security)** or **too rigid (monolithic)**.
- **Spring Boot + Java** chosen for reliability and enterprise-grade backend handling.
- **Clerk** for secure identity management (MFA, biometric login, session handling).
- **Razorpay** for verified payments and subscription management.

### 3.2 Problem Definition
Core challenge:
> Secure, decoupled file management for SaaS with reliable authentication & payments.

Key hurdles:
1. **Security Handshake:** Clerk → Spring Security token validation  
2. **File Safety:** Sanitize uploads, validate file types, prevent path traversal  
3. **Payment Integrity:** Manage Razorpay’s multi-step async flow securely

---

## 🎯 4. Objectives

### Functional Goals:
- ✅ Secure File CRUD (Create, Read, Update, Delete)
- ✅ Toggle Public/Private access
- ✅ Generate Secure Shareable Links
- ✅ Responsive UI (Grid/List view)

### Non-Functional Goals:
- 🔒 Managed Identity (Clerk)
- 🧩 Secure Authorization (Spring Security + JWT)
- 💳 Payment Integration (Razorpay + Webhooks)
- 📦 Scalable Data Model (MongoDB)

---

## ⚙️ 5. System Design & Architecture

### 🏗️ Architecture Overview

| Layer | Technologies | Description |
|-------|---------------|--------------|
| **Client (UI)** | React.js, Tailwind CSS | Handles UI, state, and API communication |
| **Server (Backend)** | Spring Boot, MongoDB | Core logic for CRUD, authorization, and payments |
| **3rd Party Services** | Clerk, Razorpay | Externalized authentication & payments for enterprise security |

---

## 🚀 6. Features

| Category | Description |
|-----------|--------------|
| **File Management** | Upload, view, download, and delete files |
| **Access Control** | Toggle file visibility (Public/Private) |
| **Secure Sharing** | Generate obfuscated, shareable links |
| **User Identity** | Clerk-managed sign-up, login, sessions |
| **Subscription** | Razorpay integration for premium features |
| **Interface** | React + Tailwind dashboard (Grid/List views) |

---

## 💡 7. Implementation Details

### 🧠 Backend Robustness (Spring Boot)
- Enterprise-grade framework for stable, type-safe code
- Strong transactional consistency for payments
- Predictable, maintainable code structure

### 🗄️ Data Persistence (MongoDB)
- Flexible document schema for dynamic metadata
- Optimized for large file dashboards and quick queries

### 🔐 Security & Authentication
1. **JWT Validation:** Clerk → Spring Security authentication pipeline  
2. **File Security:**  
   - Validate MIME type (server-side)  
   - Rename with UUIDs  
   - Store outside public web root  
3. **Payment Workflow (Razorpay):**  
   - Step 1️⃣ Order Creation (API)  
   - Step 2️⃣ Payment Verification (Webhook)  
   - Step 3️⃣ Transaction Logging (MongoDB)

---

## 🧾 8. Results & Validation

### Architectural Validation
- ⚙️ **Scalability:** Independent deployment of frontend & backend  
- 🛡️ **Security Maturity:** Enterprise authentication with Clerk  
- 💼 **Portfolio Value:** Demonstrates full-stack + SaaS-level architecture

### Feature Validation
- Secure file sharing & access toggles verified
- Razorpay integration successfully handles asynchronous transactions

---

## 🧪 9. Output / Screenshots
---
<img width="1919" height="881" alt="image" src="https://github.com/user-attachments/assets/b1707988-1bc9-40c3-b45e-997f3173b0a6" />

---

<img width="989" height="517" alt="image" src="https://github.com/user-attachments/assets/8d7f3f1d-ef4c-4f41-b9ef-6195286b2acf" />

---

<img width="1918" height="865" alt="image" src="https://github.com/user-attachments/assets/2258aa0c-3e1e-4b62-b5ec-641617bbf042" />

---

<img width="1919" height="875" alt="image" src="https://github.com/user-attachments/assets/1da93151-1941-4fd8-b638-9884384f0cf5" />

---

<img width="1091" height="841" alt="image" src="https://github.com/user-attachments/assets/262005cb-f9cb-4b51-b2be-b21d448041e8" />



---

## 🧩 10. Conclusion

The **Cloud Share** project provides:
- A **production-grade, secure full-stack architecture**
- Clean separation of concerns (React + Spring Boot + MongoDB)
- Strong emphasis on **security, scalability, and professional-grade integrations**

> ✅ Ideal as a portfolio project demonstrating **enterprise-level full-stack expertise**.

---

## 🔮 11. Future Enhancements

1. **Cloud File Storage:** Migrate to AWS S3 / Azure Blob  
2. **Config Security:** Use environment variables or Kubernetes Secrets  
3. **Reactive Backend:** Explore Spring WebFlux for non-blocking I/O  
4. **Input Validation:** Add stricter client/server-side sanitization

---




