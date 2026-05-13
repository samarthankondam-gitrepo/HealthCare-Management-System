# 🏥 HealthCare Management System

A full-stack **HealthCare Management System** developed using **Angular, Spring Boot, and MySQL**.  
This application helps hospitals and clinics manage doctors, patients, appointments, prescriptions, and user records efficiently.

---

# ✨ Features

The system provides functionalities to:

- Manage hospital operations digitally
- View doctor and patient information
- Book and manage appointments
- Generate and print prescriptions
- Manage doctor schedules and slots
- Maintain patient records securely

The application supports **3 different user roles**:

1. 👨‍💼 Admin
2. 👨‍⚕️ Doctor
3. 👤 User / Patient

---

# 👨‍💼 Admin Module

The **Admin** can perform the following operations:

- ➕ Add new doctors
- 👥 Manage users/patients
- 🩺 Manage doctors
- 📅 View available doctor slots
- 📋 View doctor, patient, and user lists
- ✅ Approve or reject doctor registrations
- 📊 Monitor overall system statistics through the dashboard:
  - Total Users
  - Total Doctors
  - Total Slots
  - Total Patients
  - Prescriptions Generated
  - Appointments Booked

---

# 👨‍⚕️ Doctor Module

The **Doctor** can perform the following operations:

- 📝 Register and login to the system
- 📋 View doctor list
- 📅 Check daily appointments
- 👥 View patient list
- ✏️ Edit doctor profile details
- ➕ Add available appointment slots
- 🕒 Manage slot schedules
- ✅ Check admin approval status
- 💊 Add patient prescriptions
- 📊 Access dashboard statistics:
  - Total Prescriptions
  - Total Doctors
  - Total Slots
  - Total Patients

---

# 👤 User / Patient Module

The **User/Patient** can perform the following operations:

- 📝 Register and login
- 👨‍⚕️ View available doctors
- 📅 Check available booking slots
- ✏️ Edit profile details
- 📌 Book doctor appointments
- ✅ Check appointment approval status
- 🖨️ View and print prescriptions
- 📊 Access dashboard statistics:
  - Total Users
  - Total Doctors
  - Total Slots
  - Total Patients

---

# 🛠️ Technologies Used

## 🎨 Frontend

- Angular
- HTML5
- CSS3
- TypeScript
- JavaScript
- Bootstrap
- jQuery
- Font Awesome
- Material UI
- Material Design Icons
- Google Fonts

---

## ⚙️ Backend

- Java
- Spring Boot
- Spring Framework
- Hibernate

---

## 🗄️ Database

- MySQL

---

# 📁 Project Structure

```bash
HealthcareManagement/
│
├── HealthcareManagement-Backend/   # Spring Boot Backend
├── HealthcareManagement/           # Angular Frontend
```

---

# 🚀 How to Run the Project

## ⚙️ Backend Setup (Spring Boot)

```bash
cd HealthcareManagement-Backend
mvn clean install -DskipTests
mvn spring-boot:run
```

Backend runs at:

```bash
http://localhost:8080
```

---

## 🎨 Frontend Setup (Angular)

```bash
cd HealthcareManagement
npm install --legacy-peer-deps
```

Optional (for OpenSSL issues):

```bash
set NODE_OPTIONS=--openssl-legacy-provider
```

Start the frontend:

```bash
npm start
```

Frontend runs at:

```bash
http://localhost:4200
```

---

# 🗄️ Database Setup (MySQL)

Create the database:

```sql
CREATE DATABASE health_db;
```

Update the `application.properties` file:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/health_db
spring.datasource.username=root
spring.datasource.password=yourpassword
spring.jpa.hibernate.ddl-auto=update
```

---

# 🌐 Access the Application

| Service | URL |
|---|---|
| Frontend | http://localhost:4200 |
| Backend API | http://localhost:8080 |
| Database | MySQL (`health_db`) |

---

# ✅ Prerequisites

Make sure the following software is installed:

- Java JDK 17
- Maven
- Node.js (v14 – v18)
- Angular CLI 12
- MySQL 8

---

# 🏗️ Build Project

Run the following command to build the Angular project:

```bash
ng build
```

Build files will be stored in the `dist/` directory.

---

# 🧪 Running End-to-End Tests

```bash
ng e2e
```

To run end-to-end tests, install the required testing packages supported by Angular.

---

# 📌 Note

- Ensure the backend server is running before starting the frontend.
- Configure the correct MySQL credentials in `application.properties`.
- Recommended to use Node.js version between 14 and 18 for compatibility.