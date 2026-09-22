# Smart Classroom Management System PRD

## Original problem statement
Build a functional and professional Smart Classroom Management System prototype for a college/school project with secure role-based login, dashboard metrics, student records, attendance, timetable, announcements, assignments, student views, notifications, reports, filtering, responsive UI, sample data, validation, loading states, and a simple understandable full-stack architecture.

## Architecture decisions
- React 19 frontend with a responsive sidebar dashboard and Axios API client.
- FastAPI backend with JWT cookie authentication and role-aware staff endpoints.
- MongoDB via the existing `MONGO_URL` and `DB_NAME` environment variables.
- Collections: users, students, attendance, timetable, assignments, announcements.
- Compact seeded demo dataset keeps the project easy to demonstrate and modify.

## Personas
- Admin/teacher: manages students, attendance, timetable, assignments, and announcements.
- Student: signs in to view classroom information, coursework, attendance, and updates.

## Core requirements
- Secure email/password login with admin and student demo roles.
- Dashboard metrics and upcoming schedule.
- Student directory with search and add flow.
- Date-based attendance marking and attendance summary.
- Weekly timetable, assignment list, announcements, and reports.
- Responsive, polished blue/green academic interface with useful states and feedback.

## Implemented — 2025-06-10
- Seeded admin/student accounts and realistic one-class sample records.
- Added JWT login/logout/session recovery and protected API access.
- Added dashboard, student directory, attendance marking, timetable, assignments, announcements, and report views.
- Added responsive navigation, search/filter surfaces, modal form validation, toast feedback, and loading/error states.

## Prioritized backlog
- P0: verify all API and browser flows after startup.
- P1: add edit/delete student actions, assignment and announcement creation forms, and student-specific dashboard filtering.
- P2: add CSV/print export, richer date filters, and notification preferences.
