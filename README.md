# 🏥 Health Care Database  

PostgreSQL Healthcare DB for managing patients, doctors, insurance & enrollments. Showcases SQL queries, design & data management skills.

## 📌 Features
- Patient records management (Name, Age, Gender, Blood Type, Medical Conditions).  
- Hospital admissions tracking (Doctor, Hospital, Room number, Billing).  
- Insurance & Plan details with premium calculations.  
- Enrollment system to link members with healthcare plans.  
- Discrepancy tracking for claim resolution.  

---

## 🛠️ Database Schema
The database contains the following tables:  

- **Members** – Patient details (name, gender, DOB, registration date).  
- **Plans** – Insurance plans with coverage type & premium.  
- **Enrollments** – Enrollment records linking members to plans.  
- **Discrepancies** – Issues raised & resolutions.  
- **Audit Log** – Tracks changes/actions for security.  

![Database ERD](Screenshot%202025-08-21%20130257.png)  

---

## 📊 Sample SQL Queries
Here are a few example queries (more in `Healthcare_enrolment.sql`):  

```sql
-- Q1: Find the total number of members
SELECT COUNT(*) AS total_members FROM Members;

-- Q2: Get all active enrollments with plan details
SELECT m.first_name, m.last_name, p.plan_name, e.status
FROM Enrollments e
JOIN Members m ON e.member_id = m.member_id
JOIN Plans p ON e.plan_id = p.plan_id
WHERE e.status = 'Enrolled';
