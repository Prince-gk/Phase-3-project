# Fitness Center Management System (CLI-Based)

## Overview
The Fitness Center Management System is a command-line interface (CLI)-based application designed to streamline the management of members, trainers, workout schedules, and membership plans in fitness centers. The system addresses common challenges in manual processes by offering structured tracking, efficient CRUD operations, and relationship management.

---

## Features
- **Trainer Management**
  - Add, view, update, and delete trainer details.
  - Track trainers' specializations and email addresses.

- **Member Management**
  - Add, view, update, and delete member details.
  - Assign members to trainers and track membership plans.

- **Schedule Management**
  - Schedule workout sessions by linking trainers and members.
  - View, update, and delete schedules.
  - Search schedules by trainer, member, or date.

- **Membership Plan Management**
  - Add, view, update, and delete membership plans.
  - Track plan durations and pricing.

- **Reports and Status Updates**
  - Mark workout sessions as "Completed" or "Missed."
  - Generate reports on trainer workload, member activity, and income from memberships.

---

## Entities and Relationships
1. **Trainers**: Trainer ID, Name, Specialization, Email.
2. **Members**: Member ID, Name, Email, Contact Number, Membership Plan, Start/End Date.
3. **Schedules**: Schedule ID, Trainer ID (FK), Member ID (FK), Workout Date, Workout Time, Activity.
4. **Membership Plans**: Plan ID, Name, Duration (Months), Price.

### Relationships
- A **Trainer** can handle multiple **Members** (One-to-Many).
- A **Schedule** links a single **Trainer** and **Member** (Many-to-One).

---

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/prince-gk/fitness-center-management.git
   ```
2. Navigate to the project directory:
   ```bash
   cd fitness-center-management
   ```
3. Install dependencies (if any):
   ```bash
   pip install -r requirements.txt
   ```
4. Run the application:
   ```bash
   python app.py
   ```

---

## Usage
1. **Main Menu:**
   - Select options to manage trainers, members, schedules, or membership plans.

2. **CRUD Operations:**
   - Use the intuitive CLI to add, view, update, or delete records.

3. **Search and Filter:**
   - Find schedules by trainer, member, or date.
   - Filter trainers by specialization or view members nearing membership expiry.

4. **Reports:**
   - Generate reports for trainer workloads and membership revenues.

---

## Future Enhancements
- Add tracking for fitness progress (e.g., weight, BMI, goals).
- Develop an online portal for members and trainers.
- Include automated reminders for membership renewals and upcoming sessions.

---

## Technologies Used
- **Language:** Python
- **Database:** SQLite
- **Interface:** Command-Line Interface (CLI)

---

## Slides
https://gamma.app/docs/Fitness-Center-Management-System-CLI-Based-06jck9c9auk25kf

## License
This project is licensed under the [MIT License](LICENSE).
