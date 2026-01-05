# 🏥 Hospital Management System — Backend

## 📘 Overview
This backend powers a **multi-role hospital management system** with role-based permissions for Super Admin, Hospital Admin, Doctor, Nurse, and Patients.  
It manages authentication, multi-tenant hospital data, appointments, prescriptions, and support tickets.

## 🛠️ Tech Stack
- **Node.js & Express.js**
- **MongoDB** (Mongoose)
- **JWT Authentication**
- **Nodemailer & SMS Integration**
- **Middleware** for role-based access and validation

## 🔄 Core Workflow
1. **Hospital Admin creates departments**  
   e.g., Cardiology, Dental, Orthopedic — each tied to a hospital.
2. **Doctor selects department** → Admin approves.
3. **Patient books appointment** → status: `PENDING`.
4. **Doctor accepts appointment** → status: `DOCTOR_ACCEPTED`  
   - Add prescription  
   - Assign nurse  
   - Complete appointment
5. **Nurse updates tasks** → status: `NURSE_ASSIGNED` → `NURSE_COMPLETED`.
6. **Doctor finalizes appointment** → `DOCTOR_COMPLETED`.
7. **Support tickets**: Patients create tickets, Admin replies, ticket auto-closes.

## 📦 Modules / Routes
- **Auth Routes**: JWT-based login & registration
- **Admin Routes**: Manage hospitals, departments, users
- **Doctor Routes**: Appointment management, prescriptions
- **Nurse Routes**: Task updates
- **Patient Routes**: Book appointments, support tickets
- **Support Routes**: Ticket system
- **Utilities**: Email, SMS, OTP, token handling

## 🔐 Key Features
- Multi-tenant system (isolated hospital data)
- Role-based access control
- Appointment lifecycle management
- Prescription flow (Doctor → Nurse → Patient)
- Support ticket system for patients
- Secure JWT-based authentication

## 🔗 Frontend Repository
[Hospital Management Frontend](https://github.com/SanjayAsokan/hospital-management-frontend)

---

