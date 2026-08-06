# 🐾 CanineAI

> A ML-powered web application that helps dog owners identify potential diseases based on symptoms and health information, while maintaining complete pet health records.

![Java](https://img.shields.io/badge/Java-21-orange?style=for-the-badge)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-4.x-brightgreen?style=for-the-badge)
![React](https://img.shields.io/badge/React-19-blue?style=for-the-badge)
![MongoDB](https://img.shields.io/badge/MongoDB-Database-green?style=for-the-badge)
![JWT](https://img.shields.io/badge/Auth-JWT-red?style=for-the-badge)

---

## 📖 Overview

CanineAI is a full-stack web application that enables pet owners to manage dog profiles, perform AI-assisted disease diagnosis, and maintain a history of health assessments.

The application provides an intuitive interface for entering symptoms, viewing prediction results, and exploring disease information through a secure and scalable architecture.

---

## ✨ Features

- 🐶 User Registration & Authentication
- 🔐 JWT-based Secure Authentication
- 👤 User Profile Management
- 🐕 Multiple Dog Profile Management
- 🧠 ML Disease Prediction
- 📊 Prediction History
- 📚 Disease Encyclopedia
- ☁️ Cloudinary Image Upload
- 📱 Responsive User Interface

---

# 🏗️ Architecture

```text
                +----------------------+
                |   React Frontend     |
                |      (Vite)          |
                +----------+-----------+
                           |
                    REST APIs (HTTPS)
                           |
                           ▼
                +----------------------+
                | Spring Boot Backend  |
                |  Business Logic      |
                +----------+-----------+
                           |
                     Spring Data
                           |
                           ▼
                +----------------------+
                |      MongoDB         |
                +----------------------+
```

---

# 📂 Project Repositories

## Frontend

**Repository**

[CanineAI Client](https://github.com/gitApurv/CanineAI-Client)

**Tech Stack**

- React 19
- Vite
- Tailwind CSS
- Axios
- React Router

---

## Backend

**Repository**

[CanineAI Server](https://github.com/gitApurv/CanineAI-Server)

**Tech Stack**

- Java 21
- Spring Boot
- Spring Security
- Spring Data MongoDB
- JWT Authentication
- Maven

---

# 🚀 Tech Stack

| Category | Technologies |
|----------|--------------|
| Frontend | React, Vite, Tailwind CSS |
| Backend | Java, Spring Boot |
| Security | Spring Security, JWT |
| Database | MongoDB |
| Image Storage | Cloudinary |
| Build Tool | Maven |
| API | REST |

---

# 🔑 Core Functionalities

### Authentication

- User Registration
- Secure Login
- JWT Authentication
- Protected Routes

### Dog Management

- Add Dogs
- Update Dog Details
- Delete Dogs
- Vaccination Tracking

### AI Diagnosis

- Select Symptoms
- Disease Prediction
- Confidence Score
- Diagnosis History

### Disease Knowledge Base

- Disease Information
- Symptoms
- Prevention Tips

---

# 🌟 Highlights

- Clean layered architecture
- RESTful API design
- Secure authentication using JWT
- Responsive React frontend
- MongoDB integration
- Modular and maintainable codebase
- Production-ready project structure
