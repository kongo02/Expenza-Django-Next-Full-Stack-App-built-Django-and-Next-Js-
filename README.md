# 📊 Finance Tracker Pro

A sophisticated, full-stack financial management application designed for precision and ease of use. It leverages a decoupled architecture, combining a **Django REST Framework (DRF)** backend with a modern **Next.js** frontend to deliver a seamless, real-time budgeting experience.

## 🚀 Key Features

* **Full CRUD Functionality:** Seamlessly add, view, and delete financial transactions.
* **Secure Data Schema:** Utilizes UUID primary keys for enhanced security and data integrity.
* **Automated Financials:** Real-time updates for Total Income, Expenses, and Net Balance.
* **Professional PDF Export:** Generate branded financial statements with category-based pie charts using `jsPDF`.
* **Categorized Tracking:** Organize spending into Food, Transport, Utilities, Entertainment, and more.
* **Secure API Communication:** Axios-driven requests with interceptors for JWT Bearer token authentication.

## 🛠️ Tech Stack

### Frontend
- **Framework:** Next.js 14 (App Router)
- **Styling:** Tailwind CSS + DaisyUI
- **Icons:** Lucide React
- **State/API:** Axios + React Hooks
- **Reporting:** jsPDF

### Backend
- **Framework:** Django & Django REST Framework (DRF)
- **Database:** PostgreSQL (Recommended)
- **Data Logic:** UUID-based models with automated timestamping

## 🏗️ Architecture



The application follows a **Decoupled Headless Architecture**:
1. **Backend (API):** A stateless REST API handling business logic and serialization.
2. **Frontend (Client):** A client-side rendered application that interacts with the API via secure interceptors.

## ⚙️ Installation & Setup

### 1. Backend Setup
```bash
cd backend
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
