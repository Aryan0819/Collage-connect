# 🎓 College Connect
### *A Full-Stack Campus Ecosystem for Clubs & Events*

<p align="center">
  <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" />
  <img src="https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white" />
  <img src="https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white" />
  <img src="https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white" />
</p>

---

## 🚀 Project Overview
**College Connect** is a robust platform built to bridge the gap between students and campus organizers. It features dedicated workflows for students to explore life on campus and for admins to govern it with precision. Built as a serverless application, it scales effortlessly on Vercel.



---

## ✨ Dynamic Features

### 🔐 Secure Authentication
* **JWT Protection**: State-of-the-art token-based security for all user sessions.
* **Role Logic**: Smart routing that distinguishes between `student` and `admin` access levels.

### 👨‍🎓 Student Experience
* **Live Event Feed**: Real-time browsing of upcoming college festivals and workshops.
* **Club Proposals**: A streamlined way for students to pitch new club ideas to the administration.
* **Join Requests**: One-click registration for approved campus clubs.

### 🛠 Administrative Power
* **Event Lifecycle**: Full CRUD (Create, Read, Update, Delete) control over the events calendar.
* **Governance**: Centralized dashboard to approve or decline club requests.
* **Data Hub**: Advanced view of registered students featuring **Live Search** and **CSV/Excel Export** capabilities.

---

## 📂 Architecture & Structure

```text
college-connect-main/
├── index.js              # Express application (Serverless entry point)
├── vercel.json           # Vercel deployment configuration
├── package.json          # Project dependencies & scripts
├── .env                  # Local environment variables (do not commit!)
└── public/               # Static frontend assets
    ├── styles/           # CSS stylesheets (login.css, etc.)
    └── pages/            # HTML views
        ├── home.html               # Main landing page
        ├── admin_events.html       # Admin: Manage/Delete events
        ├── admin_clubs.html        # Admin: Approve/Delete clubs
        ├── registrations_list.html  # Admin: Student data & CSV export
        ├── students_events.html    # Student: Event feed
        ├── students_club.html      # Student: Club directory
        └── payment.html            # QR Payment integration
```
---
## 🛠 API Reference



| Action | Route | Method |
| :--- | :--- | :--- |
| **Fetch Events** | `/events` | `GET` |
| **Admin Create** | `/admin_events` | `POST` |
| **Admin Delete** | `/admin/delete_event/:id` | `DELETE` |
| **Data Export** | `/admin/view_registrations_data` | `GET` |

---

## ⚙️ Getting Started

### ⚡ Quick Start (Local)
1. **Clone the Repo**:
   ```bash
   git clone [https://github.com/your-username/college-connect.git](https://github.com/your-username/college-connect.git)
   cd college-connect
   ```
---
### Setup Dependencies

Install the necessary packages using npm:

```bash
npm install
---
##Configure Environment
Create a .env file in the root directory and add your credentials:

```bash
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
---
## Launch Application
Start the server locally:

```bash
node index.js
---
## ☁️ Vercel Deployment
Deploying to production is seamless using the Vercel CLI. Ensure you have the Vercel CLI installed, then run:

```bash
vercel --prod
---
## 🤝 Contributing
Contributions make the open-source community an amazing place to learn, inspire, and create! Any contributions you make are greatly appreciated.

Fork the Project

Create your Feature Branch (git checkout -b feature/AmazingFeature)

Commit your Changes (git commit -m 'Add some AmazingFeature')

Push to the Branch (git push origin feature/AmazingFeature)

Open a Pull Request
---
## 📄 License
Distributed under the MIT License. See LICENSE for more information.
---
