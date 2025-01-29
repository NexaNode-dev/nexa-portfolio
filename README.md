# 🚀 Fullstack Job Board Monorepo

## 📖 Overview  
This is a **full-stack job board application** built using **Nx** to manage multiple frontends and backends in a single monorepo. It showcases different **backend implementations** (NestJS, Laravel, Rails) and **frontend approaches** (traditional SPAs and micro frontends with Angular & React).

## 🏗️ Architecture  
### **Frontend**  
- **Angular Job Board (`apps/angular-job-board`)** – Traditional Angular SPA  
- **React Job Board (`apps/react-job-board`)** – Traditional React SPA  
- **Micro Frontends (MFEs)**  
  - `apps/mfe-angular/` – Angular Shell for MFEs  
  - `apps/mfe-react/` – React Shell for MFEs  
  - `apps/mfe-job-listings/` – Job Listings MFE (Angular & React)  
  - `apps/mfe-dashboard/` – Employer/Admin Dashboard MFE (Angular)  
  - `apps/mfe-auth/` – Authentication MFE (React)  

### **Backend**  
- **NestJS API (`apps/nestjs-job-api/`)** – TypeScript backend with TypeORM  
- **Laravel API (`apps/laravel-job-api/`)** – PHP backend with Eloquent  
- **Rails API (`apps/rails-job-api/`)** – Ruby backend with ActiveRecord  
- **Shared Database** – PostgreSQL  

### **🛠️ Tech Stack**
| Layer          | Technology |
|---------------|------------|
| **Frontend**  | Angular, React, Micro Frontends (Module Federation) |
| **Backend**   | NestJS, Laravel, Rails |
| **Database**  | PostgreSQL |
| **Auth**      | JWT / OAuth |
| **CI/CD**     | GitHub Actions |
| **DevOps**    | Docker, Nx caching |

---

## 🏁 Getting Started

### **1️⃣ Install Dependencies**
```bash
yarn
```
### **2️⃣ Run the Frontends**
```bash
nx serve angular-job-board   # Angular SPA
nx serve react-job-board     # React SPA
nx serve mfe-angular         # Angular Micro Frontend Shell
nx serve mfe-react           # React Micro Frontend Shell
```
### **3️⃣ Run the Backends**
```bash
nx serve nestjs-job-api
```
(Laravel and Rails will be added later)

### **4️⃣ Run All Services in Parallel**
```bash
nx run-many --target=serve
```

### **🔥 Features & Goals**
✅ Full-Stack Architecture Comparison – NestJS vs. Laravel vs. Rails
✅ Traditional SPAs & Micro Frontends – Angular & React
✅ Modular Monorepo Setup – Nx-based multi-project management
✅ Optimized CI/CD – GitHub Actions, Docker & Nx caching

### **📌 Roadmap**
- [x] Set up Nx Monorepo ✅
- [x] Install Angular, React, and NestJS plugins ✅
- [ ] Develop NestJS backend 🚧
- [ ] Develop Angular frontend 🚧
- [ ] Develop React frontend 🚧
- [ ] Add Laravel & Rails backends
- [ ] Implement Micro Frontends (MFEs)
- [ ] Dockerize that thing

### **📜 License**
This project is licensed under the MIT License.

### **📩 Contact**
Created by Johan Vrolix <johan@nexanode.dev> and Andy Lauwers <andy@nexanode.dev> – Reach out on LinkedIn or X.
