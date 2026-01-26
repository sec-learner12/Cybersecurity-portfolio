
# **Apply Filters to SQL Queries**

## **📌 Project Description**
This project demonstrates how I used SQL filtering techniques to support security operations within my organization. As part of my role, I investigate potential security issues, analyze login activity, and identify employees who require system updates. SQL filters—using operators such as **AND**, **OR**, **NOT**, and **LIKE**—enabled me to extract precise information from the database to support these tasks.

---

## **🔍 Tasks Performed**

### **1. Retrieve After‑Hours Failed Login Attempts**
A potential security incident occurred after business hours (after 18:00).  
To investigate, I filtered the `log_in_attempts` table to return only:
- Login attempts **after 18:00**
- Attempts where **success = FALSE**

This query helped isolate suspicious failed logins occurring outside normal working hours.

---

### **2. Retrieve Login Attempts on Specific Dates**
A suspicious event occurred on **2022‑05‑09**, and activity from the day before also needed review.  
Using the **OR** operator, I filtered login attempts that occurred on:
- `2022‑05‑09`
- `2022‑05‑08`

This allowed me to quickly gather all relevant login activity surrounding the incident.

---

### **3. Retrieve Login Attempts Outside of Mexico**
Further investigation revealed unusual login attempts originating outside Mexico.  
Using **NOT** with a **LIKE** pattern (`MEX%`), I filtered for all countries **other than Mexico**, accounting for variations such as `MEX` and `MEXICO`.

This helped identify potentially unauthorized access attempts from foreign locations.

---

### **4. Retrieve Employees in the Marketing Department (East Building)**
To prepare system updates for Marketing employees, I filtered the `employees` table using:
- `department = 'Marketing'`
- `office LIKE 'East%'`

The **AND** operator ensured results included only Marketing employees located in the East building.

---

### **5. Retrieve Employees in Finance or Sales**
A separate update was required for employees in Finance and Sales.  
Using the **OR** operator, I filtered for:
- `department = 'Finance'`
- `department = 'Sales'`

This returned all employees belonging to either department.

---

### **6. Retrieve All Employees Not in IT**
To apply a final update, I needed a list of employees **not** in the Information Technology department.  
Using **NOT**, I filtered out:
- `department = 'Information Technology'`

This produced a complete list of employees outside the IT department.

---

## **🧠 Summary**
Throughout this project, I applied SQL filters to extract targeted information from two key tables:  
- `log_in_attempts`  
- `employees`

I used logical operators (**AND**, **OR**, **NOT**) and pattern matching (**LIKE** with `%`) to refine queries and support security investigations. These filtering techniques enabled efficient analysis of login activity and identification of employees requiring system updates.



