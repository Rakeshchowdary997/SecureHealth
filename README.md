# 🔐 SecureHealth — Blockchain-Based Healthcare Data Security System

> A Django-based healthcare data security application designed to manage patient records, control hospital access, and improve healthcare data integrity using blockchain concepts and MySQL.

---

## 📌 About the Project

**SecureHealth** is a web-based healthcare data management and security system developed using **Python, Django, MySQL, and Blockchain concepts**.

The main objective of the project is to provide a structured platform for managing healthcare information while controlling how hospitals access patient records.

Healthcare systems handle highly sensitive information such as patient profiles, medical conditions, contact information, and treatment-related details. SecureHealth focuses on providing controlled access to this information while using hashing and blockchain-related concepts to support data integrity.

The application provides separate workflows for patients and hospitals and allows authorized hospital users to search and access patient information according to the application's access-control logic.

---

# 🎯 Problem Statement

Traditional healthcare information systems can face challenges related to:

- Unauthorized access to patient information
- Centralized data management
- Difficulty maintaining data integrity
- Lack of controlled access between healthcare entities
- Risk of accidental or unauthorized modification
- Maintaining trustworthy records across different hospital workflows

SecureHealth explores how **Django, MySQL, access control, hashing, and blockchain concepts** can be combined to create a more structured healthcare data management application.

---

# 💡 Proposed Solution

SecureHealth provides a centralized web application where:

1. Patient profiles can be created and managed.
2. Patient information can be stored in a MySQL database.
3. Hospitals can authenticate before accessing the system.
4. Hospital users can search for patient records.
5. Patient information can be viewed through controlled workflows.
6. Access-related information can be maintained.
7. Blockchain-related hashing can be used to represent patient data integrity.
8. Sensitive application credentials are kept outside the source code using environment variables.

---

# ✨ Key Features

### 👤 Patient Management

- Create patient profiles
- Store patient information
- Maintain patient identification details
- Store medical/problem descriptions
- Maintain contact and address information
- Maintain access-control information

### 🏥 Hospital Management

- Hospital login workflow
- Controlled hospital access
- Patient search functionality
- Patient data viewing
- Access-related workflows

### 🔐 Data Security

- Environment-based database configuration
- Environment-based application secret configuration
- Environment-based hospital credentials
- Controlled access to patient information
- Hash generation for data integrity
- GitHub-safe configuration management

### ⛓️ Blockchain & Hashing

The project contains blockchain-related modules that support the generation and handling of hashes associated with healthcare information.

The purpose of this functionality is to provide a tamper-evident representation of data and support verification of data integrity.

### 💾 Database

The application uses **MySQL** for persistent storage of patient information and Django's database configuration for application-level database connectivity.

---

## ✨ Key Features

- 🔐 Secure patient record management
- 🏥 Hospital authentication and controlled access
- 👤 Patient profile creation
- 🔎 Patient record search
- 📋 Patient data viewing
- 🔑 Access control for hospital users
- ⛓️ Blockchain-based data integrity and hashing
- 💾 MySQL database integration
- 📊 Patient revenue and access tracking
- 🎨 Modern responsive web interface
- ⚙️ Environment-based configuration for sensitive credentials

## 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| Django | Web application framework |
| MySQL | Database |
| PyMySQL | Database connectivity |
| MySQLclient | Django MySQL backend |
| Blockchain | Data integrity |
| HTML | Web structure |
| CSS | User interface styling |
| JavaScript | Frontend functionality |
| Git & GitHub | Version control |

## 📂 Project Structure

```text
SecureHealth/
│
├── DataSecuring/
│   ├── __init__.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
│
├── Secure/
│   ├── Block.py
│   ├── Blockchain.py
│   ├── models.py
│   ├── views.py
│   ├── urls.py
│   ├── templates/
│   └── static/
│
├── DB.txt
├── Modules.docx
├── manage.py
├── requirements.txt
└── README.md

### 🏗️ System Architecture

```text
                    ┌───────────────────────┐
                    │       User / Hospital │
                    └───────────┬───────────┘
                                │
                                ▼
                    ┌───────────────────────┐
                    │     Django Web App    │
                    │                       │
                    │  Authentication       │
                    │  Patient Management   │
                    │  Hospital Workflow    │
                    │  Access Control       │
                    └───────────┬───────────┘
                                │
                    ┌───────────┴───────────┐
                    │                       │
                    ▼                       ▼
          ┌──────────────────┐    ┌──────────────────┐
          │      MySQL       │    │ Blockchain /     │
          │    Database      │    │ Hashing Modules  │
          │                  │    │                  │
          │ Patient Records  │    │ Data Integrity   │
          └──────────────────┘    └──────────────────┘

#🔄 Application Workflow
Patient Workflow
Patient
   │
   ▼
Patient Interface
   │
   ▼
Patient Profile
   │
   ▼
Patient Information
   │
   ▼
MySQL Database


#Hospital Workflow
Hospital
   │
   ▼
Hospital Login
   │
   ▼
Authentication
   │
   ▼
Hospital Dashboard
   │
   ▼
Search Patient
   │
   ▼
Access Patient Information
   │
   ▼
Display Patient Record

#Data Integrity Workflow
Patient Information
        │
        ▼
     Hashing
        │
        ▼
Blockchain-related Module
        │
        ▼
Integrity Representation
