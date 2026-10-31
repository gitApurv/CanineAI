# CanineAI 🐾
> An intelligent, end-to-end canine healthcare platform combining machine learning disease diagnostics, multi-pet health records, and clinical veterinary knowledge.

[![Java](https://img.shields.io/badge/Java-25-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)](https://www.oracle.com/java/)
[![Spring Boot](https://img.shields.io/badge/Spring_Boot-4.0.3-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)](https://spring.io/projects/spring-boot)
[![React](https://img.shields.io/badge/React-19.2-61DAFB?style=for-the-badge&logo=react&logoColor=black)](https://react.dev/)
[![MongoDB](https://img.shields.io/badge/MongoDB-Database-47A248?style=for-the-badge&logo=mongodb&logoColor=white)](https://www.mongodb.com/)
[![Tailwind CSS](https://img.shields.io/badge/TailwindCSS-3.4-38B2AC?style=for-the-badge&logo=tailwindcss&logoColor=white)](https://tailwindcss.com/)
[![JWT](https://img.shields.io/badge/Auth-JWT-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white)](https://jwt.io/)

---

## 📖 Overview

**CanineAI** is a full-stack, AI-powered veterinary assistance platform engineered to help dog owners track their pets' health and identify potential health conditions early. By combining user-observed clinical symptoms with machine learning inference models, CanineAI provides differential diagnoses, confidence scores, and comprehensive illness profiles while empowering owners with full medical log histories.

The platform is designed with a decoupled microservice-ready architecture comprising an enterprise Spring Boot 4 REST API, a reactive React 19 single-page application, and an upstream ML predictive pipeline.

---

## 🏛️ Ecosystem Architecture

```text
       +-------------------------------------------------------------+
       |                  Client Layer (React 19)                    |
       |  - Responsive Dashboard Layout                              |
       |  - Interactive Symptom Selector                             |
       |  - Canine Disease Encyclopedia & Filters                    |
       +------------------------------+------------------------------+
                                      |
                           HTTPS REST / Cookies / JWT
                                      |
                                      ▼
       +-------------------------------------------------------------+
       |             Backend API Service (Spring Boot 4)             |
       |  - Authentication & JWT Token Provider (Auth0)              |
       |  - Pet Management & Owner Scoping (CRUD)                    |
       |  - Symptom Catalog & Disease Knowledge Base                 |
       |  - Differential Diagnosis Aggregation Engine                |
       +--------------+------------------------------+---------------+
                      |                              |
         Spring Data Mongo Driver           REST HTTP Client
                      |                              |
                      ▼                              ▼
       +-----------------------------+ +-----------------------------+
       |     MongoDB Database        | |   ML Inference Service      |
       |  - Users & Credentials      | |  - Symptom Vectorization    |
       |  - Dog Profiles & Records   | |  - Multi-class Classifier   |
       |  - Diagnostic Audit Logs    | |  - Probability & Confidence |
       +-----------------------------+ +-----------------------------+
```

---

## ✨ Key Features

- **🐕 Multi-Pet Profile Management**: Maintain detailed digital profiles for each pet including breed, date of birth, gender, weight, profile pictures, and clinical histories.
- **🧠 Machine Learning Diagnostics**: Select observed symptoms through a categorized interface to obtain instant probability rankings and top-3 differential diagnoses.
- **📚 Verified Canine Disease Encyclopedia**: Explore clinical summaries, common symptoms, root causes, prevention guidelines, and emergency protocols across dozens of canine conditions.
- **📊 Diagnosis Audit Trail**: Comprehensive history of all previous symptom screenings with timestamps and pet mappings.
- **🔐 Enterprise-Grade Security**:
  - Stateless JWT token signing and verification
  - Secure HTTP-only cookies and Authorization header support
  - BCrypt cryptographic password hashing
  - Automated transactional email password reset workflows
- **📱 Responsive UI/UX**: Designed for mobile devices and desktops with modern aesthetics and accessible interactive elements.

---

## 📦 Project Repositories

The CanineAI ecosystem is split into dedicated, specialized repositories:

| Component | Repository Link | Description | Stack |
| :--- | :--- | :--- | :--- |
| **Backend API** | [canine-ai-server](https://github.com/gitApurv/canine-ai-server) | Core REST API, business logic, security, and MongoDB persistence | Spring Boot 4, Java 25, MongoDB, JWT |
| **Frontend Web** | [canine-ai-client](https://github.com/gitApurv/canine-ai-client) | Interactive single-page client, dashboards, and symptom selector | React 19, Vite, Tailwind CSS, Axios |

---

## 🛠️ Complete Tech Stack

| Domain | Technologies |
| :--- | :--- |
| **Frontend** | React 19, Vite 7, Tailwind CSS 3.4, React Router DOM v7, Axios |
| **Backend** | Java 25, Spring Boot 4.0.3, Spring WebMVC, Spring Security, Spring Mail |
| **Database** | MongoDB Atlas / Local Replica (Spring Data MongoDB) |
| **Authentication** | Auth0 Java-JWT, BCrypt Hashing, HTTP-only Cookies |
| **Media Hosting** | Cloudinary CDN |
| **Build & Tooling** | Maven (Backend), Vite/NPM (Frontend), Docker |

---

## 🚦 End-to-End Local Development Setup

To run the complete CanineAI platform locally:

### 1. Start MongoDB
Ensure MongoDB is running locally on port `27017` or use a MongoDB Atlas connection string.

### 2. Start the Backend API (`canine-ai-server`)
```bash
git clone https://github.com/gitApurv/canine-ai-server.git
cd canine-ai-server
# Configure src/main/resources/application.properties
./mvnw clean spring-boot:run
```
Backend initializes at: `http://localhost:8080`

### 3. Start the Frontend Client (`canine-ai-client`)
```bash
git clone https://github.com/gitApurv/canine-ai-client.git
cd canine-ai-client
npm install
npm run dev
```
Frontend runs at: `http://localhost:5173`

---

## ⚠️ Veterinary Disclaimer

CanineAI is designed as an educational and preliminary informational tool to assist pet owners. It does **not** replace professional veterinary examination, medical diagnosis, or emergency clinical treatment. Always consult a licensed veterinarian for urgent pet medical concerns.

---

## 👨‍💻 Author

**Apurv**
- GitHub: [@gitApurv](https://github.com/gitApurv)
