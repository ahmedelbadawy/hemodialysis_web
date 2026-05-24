# Hemodialysis Clinic Web App

A full-stack web application for managing a hemodialysis clinic, built with **Flask** and **SQLAlchemy**. The platform supports three user roles — **patient**, **physician**, and **admin** — each with its own dashboard and permissions, and integrates with the **Google Calendar API** to keep appointments in sync.

## Features

### Patients
- Sign in to a personal account.
- Book appointments, automatically added to their **Google Calendar** via API.
- Access their medical scans and reports online.

### Physicians
- View their appointments, synced to their own Google Calendar.
- Send reports and scans to their patients.
- Collaborate with other physicians through a built-in **blog**.

### Admins
- Full control over the platform: manage users and content, delete blog posts, and view clinic statistics.

## Tech Stack

| Layer        | Technology              |
|--------------|-------------------------|
| Backend      | Python, Flask           |
| Database/ORM | SQLAlchemy              |
| Front end    | HTML, CSS               |
| Integration  | Google Calendar API     |

## Roles & Access

| Capability                     | Patient | Physician | Admin |
|--------------------------------|:-------:|:---------:|:-----:|
| Book appointments              |   ✔     |           |       |
| Google Calendar sync           |   ✔     |    ✔      |       |
| View scans / reports           |   ✔     |    ✔      |   ✔   |
| Send reports to patients       |         |    ✔      |       |
| Physician blog                 |         |    ✔      |   ✔   |
| Manage users & content         |         |           |   ✔   |
| View statistics                |         |           |   ✔   |

## Getting Started

### Prerequisites
- Python 3.x
- A Google Cloud project with the Calendar API enabled (for appointment sync)

### Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/ahmedelbadawy/hemodialysis_web.git
   cd hemodialysis_web
   ```
2. Create a virtual environment and install dependencies:
   ```bash
   python -m venv venv
   source venv/bin/activate   # On Windows: venv\Scripts\activate
   pip install -r requirements.txt
   ```
3. Configure the Google Calendar API credentials (add your `credentials.json` / API keys as required).
4. Run the app:
   ```bash
   python app.y
   ```
5. Open the app in your local host.
