# Unified Grievance Intelligence & Resolution Platform (UGIRP)

A modern, enterprise-ready full-stack civic resolution dashboard. UGIRP is built on a responsive React (Vite) frontend with a highly secure NodeJS + Express + MongoDB backend.

## Features

* **Citizen Experience:** AI-driven auto-categorizing complaint forms, visual ETA timelines, and full ticket tracking.
* **Officials Workspace:** Authorized workers have a Kanban grid to securely Claim, Resolve, and Release active tickets.
* **Admin Analytics Space:** Top-tier dashboard powered by interactive `recharts`, visualizing category volumes, timeline analytics, and enabling 1-click User Role promotions.
* **Role-Based Access Control (RBAC):** Backend Express middleware tightly isolates endpoints based on strictly enforced `JWT` payload roles (`citizen`, `officer`, `admin`).
* **Robust Engine:** Offline-capable architecture temporarily utilizing `mongodb-memory-server` ensuring an ultra-fast local sandbox.

## Quick Start

### 1. Initialize the Server Pipeline
```bash
cd server
npm install
npm run dev
```
> **Note:** The backend operates natively on `http://localhost:5000`. By default, it auto-seeds a master administrator logic login right on startup: 
> **Email:** `admin@ugirp.local` | **Password:** `admin123`

### 2. Initialize the Client React Bundle
```bash
cd client
npm install
npm run dev
```
> **Note:** Access the frontend web app on `http://localhost:5174`.

## Tech Stack
* **UI Structure:** React 18, Vite, Tailwind CSS, Lucide-React, Framer-Motion.
* **Analytics Component:** Recharts.
* **API Flow & Storage:** Express.js, Mongoose/MongoDB, JSON Web Tokens (JWT), Bcrypt hashing.
