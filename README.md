# 🩸 Blood Bank Management System

A full-stack web application built with **Python and Django** to manage blood donors, blood inventory and blood requests in one place. It has role-based access for three types of users (**Admin, Donor and Patient**) and an interactive dashboard that shows up-to-date blood availability across all blood groups.

---

## 📌 Overview

Blood banks often track donors, stock and requests in separate registers or spreadsheets, which makes it hard to know what is available when someone urgently needs blood. This project puts everything into a single system:

- Donors can register and keep their details up to date.
- The blood inventory is tracked by blood group.
- Patients can request blood, and admins manage those requests.
- A live dashboard shows current availability at a glance.

---

## ✨ Features

**Role-based access**
- **Admin:** manages donors, blood inventory and incoming blood requests, and views the dashboard.
- **Donor:** registers, logs in and manages their own profile and donation details.
- **Patient:** registers, logs in and submits blood requests.

**Core functionality**
- Donor registration and record management
- Blood inventory tracking by blood group
- Blood request workflow from submission to admin action
- Interactive **ApexCharts** dashboard showing blood availability across blood groups
- Responsive UI built with Bootstrap

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|------------|
| Backend | Python, Django |
| Frontend | HTML, CSS, JavaScript, Bootstrap |
| Charts | ApexCharts |
| Database | SQLite (default) |

---

## 📸 Screenshots

<!-- TODO: add your screenshots to a docs/screenshots folder and update the file names below -->

| Login | Admin Dashboard |
|-------|-----------------|
| ![Login](docs/screenshots/login.png) | ![Admin Dashboard](docs/screenshots/admin-dashboard.png) |

| Donor Registration | Blood Request |
|--------------------|---------------|
| ![Donor Registration](docs/screenshots/donor-registration.png) | ![Blood Request](docs/screenshots/blood-request.png) |

---

## ⚙️ Installation

**Prerequisites:** Python 3.10 or newer and Git.

```bash
# 1. Clone the repository
git clone https://github.com/Anuraj00/BloodBank-System.git
cd BloodBank-System

# 2. Create and activate a virtual environment
python -m venv venv
source venv/bin/activate        # On Windows: venv\Scripts\activate

# 3. Install dependencies
pip install -r requirements.txt

# 4. Apply database migrations
python manage.py migrate

# 5. Create an admin account
python manage.py createsuperuser

# 6. Start the development server
python manage.py runserver
```

Then open **http://127.0.0.1:8000/** in your browser.

---

## 🚀 Usage

1. Log in with the admin account you created to reach the admin dashboard.
2. Register as a **Donor** or **Patient** from the sign-up page to try the other roles.
3. As a patient, submit a blood request. As an admin, review it and update the inventory.
4. Open the dashboard to see blood availability by group.

---

## 🗄️ Database Design

The relational schema covers donors, blood inventory by blood group, and blood requests, linked to the three user roles. Django's ORM and migrations manage the tables.

<!-- TODO (optional but recommended): add an ER diagram image here, e.g. ![ER Diagram](docs/er-diagram.png) -->

---

## 🔮 Future Improvements

- REST API for mobile or third-party integration
- Email/SMS notifications for urgent requests
- Fully mobile-responsive layouts
- Deployment with a production database (PostgreSQL)

---

## 👤 Author

**Anuraj Kumar**
- GitHub: [@Anuraj00](https://github.com/Anuraj00)
- Email: anurajkumar0805@gmail.com
