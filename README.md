# 📊 Research Projects Database (SQL)

This project demonstrates a relational database design for managing **research projects**, including associated employees, project managers, funding agencies, and employee-project assignments.

---

## 🧱 Entity-Relationship Overview

This database supports the following real-world scenario:

- **Projects** are conducted under a **single funding agency**.
- Each **project** has a **unique name within the agency**, a **budget**, **duration**, and a **manager** (who is also an employee).
- **Employees** (with SSNs) can work on multiple projects.
- **Managers** are also included in the employee list.
- Each **funding agency** has a unique ID, name, and address.



## 📌 Notes

- Project names are assumed to be unique within a funding agency (not enforced in schema).
- Duration is stored as integer (e.g., months).
- `Employee_Project` can be extended with roles, hours, etc.
- Currently, projects are not directly linked to `FundingAgency` in the schema but can be added using a `Agency_ID` foreign key in the `Project` table if needed.

---

## ✅ Future Enhancements

- Add `Agency_ID` to the `Project` table.
- Normalize project names within agency scope.
- Add project roles, assignment dates, and contribution percentages.

---

## 🛠️ Technologies Used

- SQL (PostgreSQL/MySQL compatible syntax)
- Relational Database Modeling

---

## 📎 License

This project is for educational/demo purposes.
