# Municipal Assessor's Office - Document Request & Verification System

A Python-based console application designed for municipal assessors' offices.
It provides a multi-role platform for **Residents** to register, log in, request documents, book appointments, and track requests, as well as for **Staff** to monitor, verify, review, and update document request statuses.

Features

Main Menu

* Resident Portal — Access resident authentication and dashboard features
* Staff Portal — Secure portal for staff verification and management functions
* Exit System — Safely closes the application with a polite exit message

Resident Portal & Dashboard

1. Log In / Create Account — Unique account registration with duplicate username checks
2. Submit Document Request — Submit requests with property owner details and reference tracking
3. My Requests and Appointments — View a personalized list of all submitted requests
4. View Available Documents — Check accessible assessor certificates and records
5. Book / Cancel Appointment — Manage schedule slots for physical processing or claiming

Staff Menu & Verification Workflow

1. Request Monitoring — Review all pending and submitted document requests across residents
2. Verify Requirements — Verify resident documents and check requirement completeness
3. Resume Request Review — Process and update requests marked as *Action Required*
4. Update Request Status — Dynamically change statuses (e.g., *Under Review*, *Action Required*, *Completed*)

Default Staff Credentials

Role | Username | Password
--- | --- | ---
Staff / Admin | admin | 123

How to Run

1. Make sure you have Python 3 installed.
2. Save the code as a `.py` file (e.g. `assessor_system.py`).
3. Run it in your terminal / command prompt:

```bash
python assessor_system.py

or

python3 assessor_system.py

Key Behaviors

1. Multi-Role Portals: Distinct functional pathways for public residents versus internal municipal staff.
2. Verification Tracking: Tracks multi-state requests, including requirement checks and note updates for missing items.
3. Duplicate Account Prevention: Prevents multiple registrations using the same username.
4. Reference Numbering: Automatically tracks and updates global request reference numbers throughout user sessions.

Project Structure (Single File)
All data is managed in memory using lists and standard data structures:

1. resident_accounts — Stores registered resident user data [username, password, name]
2. requests — List containing all submitted request details, requirement notes, and statuses
3. resident_dashboard() — Main hub for resident-side actions and appointment management
4. staff_menu() — Dedicated interface for administrative request processing and verification workflows

No external database or third-party packages required — runs purely on Python standard libraries.
Notes

1. Data Persistence: Data is kept in-memory and will reset upon program exit.
2. Interface: Text-based Command Line Interface (CLI).
3. Intended for classroom project demonstrations, workflow simulations, and local government unit (LGU) system prototypes.

Author

Created as a student project.
Feel free to fork, enhance, or add file/database saving functionality!
