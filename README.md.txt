
# 💰 Expense Management System

The Expense Management System is a web application built with Angular that helps users manage shared expenses within groups. It ensures transparency by automatically calculating how much each user owes or is owed, while supporting secure authentication and role-based access.


---

## 🚀 Features

1. 👥 Group Management: Create groups and add members.

2. 💵 Expense Tracking: Add expenses and view all groups you are part of.

3. ⚖️ Auto Balance Calculation: System automatically calculates how much each user owes.

4. 🔐 Authentication: JWT-based login & route protection.

5. 🛡️ Roles: Supports both Admin and User roles.

6. ⚠️ Error Handling: Exceptions managed using Angular HTTP Interceptor.

7. 📱 PWA Support: Configured with ngsw-config.json for service worker support.



---

## 🏗️ Project Structure

The app follows a feature-first structure with clear separation of concerns:

Auth → JWT-based authentication, middleware for protecting routes.

Backend →

1. server.js → Express API.

2. authMiddleware.js → Security.

3. serverData.json → Mock persistence.


Group → Create groups & list user groups.

Expense → Add expenses, calculate balances.

Core → HTTP interceptor & authentication guards.

Shared → Reusable Angular components, services, and utilities.

Build/Deploy → Production build artifacts inside dist/expense-tracking-project.

Routing → Authentication, group listing, and expense logging with guards.



---

## 🛠️ Installation & Setup

1️⃣ Clone the Repository

git clone <repository_url>
cd expense-management-system

2️⃣ Install Dependencies

npm install

3️⃣ Run in Development Mode

Start Angular app:

ng serve

Start JSON Server:

npm run json


4️⃣ Run Production Build

Build Angular app:

ng build --prod

Start server with production build:

node server.js



---

👩‍💻 Tech Stack

Frontend: Angular

Backend: Node.js + Express

Authentication: JWT

Persistence: JSON Server (Mock Database)

Deployment: Runs from dist/expense-tracking-project



---

👨‍👩‍👧‍👦 Team Members

Sairaj Rajput

Harshita Mahajan

Ankur Pandey

Sapna Rani



---

🔒 Security

Token-based authentication on all API endpoints.

Route guards for feature modules.

Middleware for backend request validation.
