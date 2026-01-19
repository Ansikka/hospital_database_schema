**🏥 Hospital Readmission Analysis System**

**📌 Project Overview**

This project implements a Hospital Database Management System using Python and SQLite to analyze patient readmission rates and identify the department responsible for patient care.
It is designed for academic DBMS projects, healthcare analytics, and exam demonstrations.

🎯 Objectives

Store hospital data in a structured relational database

Track patient readmissions

Identify patients with the highest readmission rates

Determine the department and doctor responsible for care

Use synthetic (random) data to maintain privacy

🧩 Database Schema
📋 Tables Included
1️⃣ Patient
Column	Description
PatientID	Primary Key
PatientName	Patient full name
Age	Age of patient
Gender	Male/Female
Disease	Diagnosed disease
BloodGroup	Blood group
Phone	Contact number
City	City of residence
2️⃣ Department
Column	Description
DepartmentID	Primary Key
DepartmentName	Department name
3️⃣ Doctor
Column	Description
DoctorID	Primary Key
DoctorName	Doctor name
DepartmentID	Foreign Key (Department)
4️⃣ Readmission
Column	Description
ReadmissionID	Primary Key
PatientID	Foreign Key (Patient)
DepartmentID	Foreign Key (Department)
DoctorID	Foreign Key (Doctor)
ReadmissionDate	Date of readmission
🔁 Relationships

One Patient → Many Readmissions

One Department → Many Doctors

One Doctor → Many Readmissions

Readmission links Patient, Doctor, and Department

⚙️ Technologies Used

Python 3

SQLite

sqlite3 (database handling)

random, datetime (synthetic data generation)

🚀 Features Implemented

Creation of hospital database tables

Generation of random Indian patient data

Simulation of readmission events

Query to identify:

Patient with highest readmission rate

Department(s) responsible for care

Clean relational design with foreign keys

▶️ How to Run

Open the provided Python file / notebook

Run all cells or execute the script

SQLite database (hospital.db) will be created automatically

Output will display:

Patient with highest readmission

Responsible department(s) and doctor(s)

📊 Sample Output
Patient with highest readmission: Riya Singh (ID: 3), Count: 8
Department: Pulmonology, Doctor: Dr. Riya Verma
Department: Cardiology, Doctor: Dr. Arjun Singh

**🧠 Use Cases**

DBMS lab assignments

Healthcare analytics projects

Hospital information systems

Interview / viva demonstrations

Data modeling practice (ERD → Tables)

**🔐 Data Privacy**

All patient data is synthetically generated.
No real patient information is used.

**📌 Future Enhancements**

Appointment table integration

Billing and insurance analysis

Visualization (Excel / charts)

ML-based readmission prediction

✍️ Author
Anshika Sharma
