# Health Care Data Management System — My Contribution

**Academic work** — CPSC 5071 Data Management for Data Science, Seattle
University, Winter 2025. A group project with Devi Sowjanya Padala, Naveen
Pasupula, and me — and I contributed to most parts of it.

This is my write-up of the project and the work I did in it. The milestone
documents were our group's shared write-ups, so they're not in this repo.

## What the project was

We designed and built a database system for running a hospital: patient
records, appointments, lab reports, billing, and patient feedback. It covers
patients, employees, departments, appointments, diseases, lab tests, billing,
and feedback, with a small desktop app on top and a Tableau dashboard for
looking at the data.

## What I contributed

I worked across most of the project with the team — the SQL queries, the data
work behind them, and the app and dashboard we built on top.

- **The queries.** The queries in this repo pull the useful stuff out of the
  database — patient visit history, appointments with the doctors and roles
  assigned to them, lab reports, billing, and how doctors were doing based on
  patient feedback. They join across the patient, appointment, employee,
  disease, lab test, billing, and feedback tables.
- **The data work.** The database itself is a normalized design across the
  hospital's entities — patients, addresses, employees and their roles,
  departments, appointments, diseases, lab tests, billing, and feedback — and
  I worked with the team on getting the data into that shape.
- **The app and the dashboard.** We also built a small Tkinter desktop app
  (login with role-based access — doctors, surgeons, and patient care
  technicians see different things) and a Tableau workbook with dashboards on
  the hospital data. The app's database connection is blanked out here — put
  your own credentials in to run it.

## Tools

MySQL (MySQL Workbench data model), SQL, Python (Tkinter, mysql-connector),
Tableau.

## What is not here

- The milestone documents and the final presentation were the group's shared
  write-ups, so they're not here — this write-up covers my part instead.
- The datasets are not included. We made up the patient, employee, and
  appointment records for the course, but they're written to look like real
  personal records — names, dates of birth, phone numbers, emails, even
  passwords. Even though the data is made up, I'm not putting files like that
  online.
- The per-person data dumps are not included either, for the same reason.

## How to run it

1. Create the database from `HospitalManagement_DBModel.mwb` in MySQL
   Workbench.
2. Run the queries in `HealthCareData_Queries.sql` against your own database.
3. In `milestone3.py`, set the host, user, password, and database to your own
   MySQL connection, then run it with Python 3.
