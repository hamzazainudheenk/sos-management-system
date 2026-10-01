<div align="center">

<img src="logo.png" alt="School of Skills Logo" width="260"/>

# 🏫 SOS — School of Skills Management System

**A modern, easy-to-use school management dashboard built with Python and Streamlit.**
Manage staff, programs, students, attendance and fees — all in one place.

![Python](https://img.shields.io/badge/Python-3.9%2B-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-Dashboard-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data-150458?style=for-the-badge&logo=pandas&logoColor=white)
![OOP](https://img.shields.io/badge/Concept-OOP-DC2626?style=for-the-badge)

</div>

---

## 📖 About The Project

**School of Skills (SOS)** is a skill-training institute based in **Calicut, Kerala**.
This project is a complete **management system** for the school. It helps the admin desk
do daily work like enrolling students, marking attendance, collecting fees and
posting notices, without any paper or spreadsheets.

The project is split into two clean parts:

| File | What it does |
|------|--------------|
| `sos.py` | The **brain**. It has all the classes and rules (no screen code). |
| `app.py` | The **face**. It builds the screens, colors and buttons using Streamlit. |

---

## ✨ Features

### 🏠 Home
- Beautiful red & white hero banner with the school logo
- Live notice board (add notices as **General, Urgent, Event or Exam**)
- Quick overview cards of the whole school

### 🏫 School Details
- School profile: name, location, established year, contact, email, website and affiliation

### 👥 Staff
- View all staff with a **role filter**
- Add new staff: **Teacher, Student Coordinator, Media Team, Accountant**
- **Trash bin** to restore or permanently delete staff

### 🎓 Programs
- View all courses with duration, fees and the faculty lead
- Add new programs by department: **Tech, Business, Design, Media**
- Assign or change the teacher of a program
- **Trash bin** for removed programs

### 👨‍🎓 Students
- View students with filters by **program, batch and fee status**
- Enroll a student into a program with batch, teacher, date and total fees
- **Trash bin** for removed students

### ✅ Attendance
- **Student attendance:** mark one by one or in **bulk by program and batch**
- **Staff attendance:** mark present or absent for each staff member
- Attendance percentage is calculated automatically

### 💰 Fees
- Collect fees using **UPI / GPay, Cash, Debit / Credit Card or Net Banking**
- Auto-generated receipts like `REC-2026-1234`
- Full **payment history** for every student
- Fee status badges: **Fully Paid, Partially Paid, Unpaid**

### 📊 Analytics
- **Fee recovery:** total billed, collected, pending and recovery rate
- **Attendance:** students with 75% or more vs. below 75%, and average attendance per class
- **Enrollment:** which programs have the most students

---

## 🛡️ Smart Rules Built In

The system protects the admin from common mistakes:

- A student **cannot join two programs** at the same time
- Attendance and fees are **only allowed for enrolled students**
- A fee payment **cannot be zero or negative**
- A fee payment **cannot be more than the amount due**
- A student who has already paid in full **cannot be charged again**

---

## 🧠 OOP Concepts Used

This project is also a good example of Object-Oriented Programming in Python:

| Concept | Where it is used |
|---------|------------------|
| **Abstract Base Class** | `SOS` is the parent idea for the whole school |
| **Inheritance** | `Teacher`, `StudentCoordinator`, `MediaTeam`, `Accountant` inherit from `Staff` |
| **Encapsulation** | Private fields like fees, batch and attendance inside `Student` |
| **Class Variables** | School name, location and director shared by all objects |
| **Class Methods** | `display_all_students()`, `search_staff()`, `display_trash()` |
| **Controller Class** | `SOSActivities` handles workflows like enrolling and collecting fees |

---

## 🗂️ Project Structure

```
School-of-Skills/
│
├── app.py             # Streamlit user interface (screens, styling, pages)
├── sos.py             # Business logic (classes and rules, no UI code)
├── logo.png           # School logo
├── requirements.txt   # Python packages needed
└── README.md          # You are here
```

---

## 🚀 How To Run It On Your Computer

**1. Clone the project**
```bash
git clone https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git
cd YOUR-REPO-NAME
```

**2. Install the packages**
```bash
pip install -r requirements.txt
```

**3. Start the app**
```bash
streamlit run app.py
```

**4. Open your browser** at `http://localhost:8501` 🎉

---

## 🧪 Sample Data

When you open the app for the first time, it loads **sample data** so you can try
everything right away:

- 🎓 **5 programs:** Data Scientist & Analyst, Human Resource, Fashion Design, AI - Agent K, Spoken English
- 👩‍🏫 Sample teachers and staff
- 👨‍🎓 **14 sample students**
- 📢 1 sample notice

> ⚠️ **Note:** Data is stored in memory only. When you restart the app, it goes back to the sample data.

---

## 🛠️ Built With

- [Python](https://www.python.org/) — main language
- [Streamlit](https://streamlit.io/) — web dashboard
- [Pandas](https://pandas.pydata.org/) — tables and charts data

---

## 🔮 Future Ideas

- [ ] Save data permanently using a database (SQLite / PostgreSQL)
- [ ] Admin login system
- [ ] Download fee receipts as PDF
- [ ] Export reports to Excel
- [ ] SMS / WhatsApp reminders for pending fees

---

## 🤝 Contributing

Ideas and improvements are welcome!

1. Fork this repo
2. Create your branch: `git checkout -b feature/my-idea`
3. Commit your changes: `git commit -m "Add my idea"`
4. Push it: `git push origin feature/my-idea`
5. Open a Pull Request

---

## 📬 Contact

**School of Skills** — Calicut, Kerala, India
🌐 [schoolofskills.com](https://schoolofskills.com) • ✉️ info@schoolofskills.com

---

<div align="center">

⭐ **If you like this project, please give it a star!** ⭐

Made with ❤️ using Python & Streamlit

</div>
