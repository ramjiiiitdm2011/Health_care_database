Health Care Database

This project is a PostgreSQL-based healthcare database system designed to efficiently manage patient information, medical records, insurance plans, and hospital data. The database schema captures key aspects of healthcare operations, ensuring data consistency, scalability, and reliability for healthcare analytics and applications.

📌 Features

Patient Information Management – Stores member details such as name, age, gender, and date of birth.
Medical Records Tracking – Maintains health-related information including blood type, medical conditions, doctors, hospitals, and billing.
Insurance & Plans – Manages insurance providers, plan details, coverage types, and premiums.
Enrollments – Tracks member enrollments into specific healthcare plans.
Discrepancy Management – Logs and resolves discrepancies related to insurance or healthcare services.
Audit Logging – Maintains system activity logs for monitoring and compliance.

🗄️ Database Schema

The database contains the following main tables:
members – Stores patient demographic details.
health_data – Captures patient medical and hospital-related information.
plans – Contains insurance plan details.
enrollments – Connects members to their respective insurance plans.
discrepancies – Records issues and resolutions in healthcare services.
audit_log – Tracks user actions for accountability.

🎯 Use Cases

Healthcare providers can manage patient admissions and billing.
Insurance companies can handle plan enrollments and claims.
Administrators can monitor discrepancies and maintain audit trails.
Data analysts can use this system for healthcare analytics and reporting.

🛠️ Tools & Technologies

Database: PostgreSQL 17
Interface: pgAdmin 4
Schema Design: ERD with relational integrity

Interface: pgAdmin 4

Schema Design: ERD with relational integrity
