# Health Care Data Management System

My group project from CPSC 5071 Data Management for Data Science, Seattle
University, Winter 2025. I built it with Devi Sowjanya Padala and Naveen
Pasupula, using MySQL, Python, and Tableau.

## What this project is

We designed and built a database system for running a hospital: patient
records, appointments, lab reports, billing, and patient feedback. It covers
patients, employees, departments, appointments, diseases, lab tests, billing,
and feedback, with a small desktop app on top and a Tableau dashboard for
looking at the data.

## What I worked on

My write-up of the project and my part in it is in
`Healthcare_Data_Management_My_Contribution.md`. I contributed to most parts
of this one — the SQL queries, the data work, and the app and dashboard with
the team.

## Files

- `Healthcare_Data_Management_My_Contribution.md` — my write-up of the
  project and the work I did in it
- `HealthCareData_Queries.sql` — the queries (the database name is generic
  here so it runs against your own database)
- `milestone3.py` — the Tkinter desktop app: login with role-based access,
  then a query page. The database login is blanked out — put your own
  credentials in to run it.
- `HospitalManagement_DBModel.mwb` — the MySQL Workbench data model
- `Healthcare_Tableau_Workbook.twbx` — the Tableau dashboard workbook (the
  course database connection details are taken out, so the dashboards are
  there but it won't connect on its own)

## What is not here

- The milestone documents and the final presentation were our group's shared
  write-ups, so they're not here — my write-up above covers my part instead.
- The datasets are not included. We made up the patient, employee, and
  appointment records for the course, but they're written to look like real
  personal records — names, dates of birth, phone numbers, emails, even
  passwords. Even though the data is made up, I'm not putting files like that
  online. Same for the per-person data dumps.
- The app used to connect to our course database, so it won't run without a
  university account anyway.

## How to run it

1. Create the database from `HospitalManagement_DBModel.mwb` in MySQL
   Workbench.
2. Run the queries in `HealthCareData_Queries.sql` against your own database.
3. In `milestone3.py`, set the host, user, password, and database to your own
   MySQL connection, then run it with Python 3.

## Tools

MySQL (MySQL Workbench data model), SQL, Python (Tkinter, mysql-connector),
Tableau.
