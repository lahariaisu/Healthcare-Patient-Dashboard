
# 📊 Hospital Patient Dashboard

This project is an interactive **Hospital Patient Dashboard** built using **Power BI**. It helps hospital staff and management easily track patient details, medicine sales, hospital charges, and daily medicine usage.

---

## 📌 Project Overview

**Key Features:**
- View **patient details** such as name, age, doctor, and diagnosis.
- Track **admission and discharge dates**.
- Monitor **total bill amounts** and **medicine sales (quantity)**.
- Analyze **daily and monthly medicine usage**.
- Visualize **medicine sales breakdown** by type.
- Breakdown **patient charges** by charge type (tests, doctor fee, admission, etc.).
- Integrated with a **data model** containing tables for patients, appointments, tests, medicines, hospital bills, and calendar.

---

## 🗂️ Data Model

The dashboard uses a well-structured relational data model with the following key tables:

- **Patient:** Stores patient demographics, admission status, bed details.
- **Appointment:** Tracks appointment dates, doctors, fees, and diagnosis.
- **Patient_tests:** Contains test results, test categories, and amounts.
- **Medical Stock:** Maintains medicine details like batch number, category, cost price, and stock quantity.
- **Medicine_Patient:** Links patients with medicines prescribed and dispensed.
- **Hospital Bills:** Stores detailed billing information by charge type.
- **Calendar:** A date dimension table for time-based analysis.
- **_Measures:** Holds DAX measures for `Total Bill Amount` and `Medicine Sale (QTY)`.

---

## ⚙️ Dashboard Visuals

| Section | Description |
|-----------------|---------------------|
| **Patient List** | Filter to select and view individual patient records. |
| **Patient Details** | Displays selected patient's age, doctor, and diagnosis. |
| **Admission/Discharge Dates** | Admission date shown; discharge date blank if still admitted. |
| **KPIs** | Shows total bill amount (`56K`) and total medicine sales (`134` units). |
| **Medicine Usage Heatmap** | Shows medicine tracking by month and day. |
| **Medicine Sales Bar Chart** | Ranks medicines by quantity dispensed. |
| **Patient Charges Breakdown** | Visualizes charges by type (e.g., admission, doctor fee, tests). |

---

## 🧩 Relationships

- **Patient** is the core table linked with **Appointments**, **Patient_tests**, **Hospital Bills**, and **Medicine_Patient**.
- **Medicine_Patient** is connected to **Medical Stock** to fetch medicine details.
- **Calendar** is linked to **Medicine_Patient** and **Hospital Bills** for date-based slicing.

---

## 🧮 Measures

Key DAX measures:
- **Total_Bill_Amt:** Calculates the total hospital bill amount.
- **Medicine Sale (QTY):** Sums the total quantity of medicines dispensed.

---

## 🧑‍💻 Tools & Tech

- **Power BI Desktop**
- DAX for custom measures
- Relational data model design
