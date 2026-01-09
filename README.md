# Soyle-Cafe-Management-System
Soyle | Next-Gen Café Operating System. An end-to-end hospitality solution featuring QR mobile ordering, real-time Kitchen Display System (KDS), and inventory analytics. Built on a high-concurrency Microservices architecture (Go + React).
# Next-Generation Cafe Order Management System

> **"Taste at its fastest."**
> [**View Live Product Demo & Landing Page**](https://order-system-soyle.vercel.app)
> * **Promotional Site:** [soylead.carrd.co](https://soylead.carrd.co/)

---

## Executive Summary

**Soyle** is a comprehensive SaaS solution designed to digitize the operational workflow of cafés and restaurants. Addressing the critical pain points of manual order taking, inventory inefficiencies, and kitchen communication errors, Soyle provides a seamless, QR-based ecosystem.

Unlike traditional POS systems requiring expensive proprietary hardware, Soyle operates on a **BYOD (Bring Your Own Device)** model with a cloud-native architecture, ensuring zero setup costs for venue owners and an app-free experience for customers.

---

## Architecture & Design Philosophy

we implemented a Modular Monolith architecture. We didn't just build a web app; we engineered a high-performance operating system for restaurants. Our architectural choices were driven by the need for **low latency**, **high concurrency**, and **cost efficiency** during peak operational hours. 


> 📂 **Deep Dive:** For comprehensive details on our Database Schema, CI/CD Pipelines, and API Contracts, please refer to the technical documents in the `docs/` directory.

### Core Technology Stack
* **Backend:** Golang (Fiber Framework) – Selected for high concurrency and low-latency API responses.
* **Frontend:** React.js (Vite) – Delivers a reactive Single Page Application (SPA) experience.
* **Database:** PostgreSQL (Neon Tech) – Relational data integrity for financial transactions and inventory.
* **Real-Time Sync:** WebSocket Protocol – Powering the instant synchronization between Customer Orders and the Kitchen Display System (KDS).

### DevOps & Infrastructure
* **Containerization:** Fully Dockerized services ensuring consistency across Development and Production environments.
* **CI/CD Pipeline:** Automated GitHub Actions workflows that trigger parallel deployments to Vercel (Frontend) and Render (Backend) upon code push.
* **Security:** Enforced CORS policies, JWT Authentication, and strict Role-Based Access Control (RBAC).

---

## Modules & Key Features

The ecosystem consists of **four** synchronized interfaces designed to cover every aspect of the operation:

### 1. Customer Experience (QR Web App)
* **Instant Ordering:** Scan QR, browse the menu, and order without downloading an app.
* **Hybrid Payment & Loyalty:** Pay online (Credit Card) or at the cashier. Earn/spend loyalty points with every order.
* **Interactive Feedback:** Customers can leave star ratings and comments directly through the app.
* **Order History:** Logged-in customers can view their past orders.

### 2. Cashier (POS) Panel
* **Table Management:** View all active tables and their instant order status.
* **Payment Processing:** Handle cash/card settlements and track discounted orders (Loyalty points usage).
* **Order Closure:** Close tables and finalize transactions with a single click.

### 3. Kitchen Display System (KDS)
* **Real-Time Workflow:** Orders appear instantly via WebSockets, prioritizing new items.
* **Status Updates:** Chefs can mark orders as "Prepared" or "Completed" to notify the staff.
* **Archive:** Access to past completed orders for kitchen efficiency analysis.

### 4. Admin & Operations Dashboard
* **Menu Management:** Add, edit, or delete products and prices in real-time.
* **Stock Tracking:** Monitor critical stock levels; items automatically update based on availability.
* **Review Moderation:** View and delete customer feedback to maintain quality control.
* **Sales Reports:** Track daily revenue and completed orders.
  
---

## Team Ventus

Soyle was architected and developed by my team.

* **Muhammet Ali Öztürk** – *Team Lead & Scrum Master*
* **Oğuzhan Şükrü Keleş** 
* **Nihat Avcı** 
* **Mehmetali Açık** 
* **Muhammed Osman Kara**

---

## Contact & Investment

Soyle has completed its MVP phase and is currently live. We are open to investment opportunities to scale our operations.

* **Email:** [ozturkmuhammetali395@gmail.com]
* **LinkedIn:** [http://linkedin.com/in/muhammet-ali-%C3%B6zt%C3%BCrk-6a4577337]

---
*© 2025 Soyle. All Rights Reserved. Source code is held in private repositories for intellectual property protection.*
