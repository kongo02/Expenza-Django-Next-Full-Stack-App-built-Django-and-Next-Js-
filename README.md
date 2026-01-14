# 📊 Finance Tracker Pro

A high-performance, full-stack financial management application designed for precision and clarity. This project features a decoupled architecture, combining a **Django REST Framework (DRF)** backend with a modern **Next.js** frontend to deliver a seamless, real-time budgeting experience.


## 🚀 Key Features

* **Real-Time Analytics:** Instant calculation of Total Income, Expenses, and Net Balance via React state management.
* **Data Visualization:** Interactive spending breakdown by category using **Recharts** with custom-themed UI.
* **Professional PDF Engine:** A custom-built **jsPDF** implementation that generates branded financial statements, including a dynamically rendered Canvas-based pie chart and running balance calculations.
* **Categorized Tracking:** Advanced categorization (Food, Transport, Utilities, Entertainment, Other) with color-coded visual cues.
* **Secure API Architecture:** * **Frontend:** Axios-driven requests with interceptors for JWT Bearer token authentication and local storage persistence.
    * **Backend:** UUID-based data modeling for enhanced security and non-predictable resource URIs.
* **Modern UI/UX:** Built with **Tailwind CSS** and **DaisyUI**, featuring a sleek "Night Mode" theme and responsive design for mobile/desktop.

## 🛠️ Tech Stack

### Frontend
- **Framework:** Next.js 15 (App Router)
- **Visualization:** Recharts (SVG) & HTML5 Canvas (for PDF)
- **Styling:** Tailwind CSS + DaisyUI
- **Icons:** Lucide React
- **Notifications:** React Hot Toast
- **PDF Generation:** jsPDF

### Backend
- **Framework:** Django & Django REST Framework (DRF)
- **Database:** PostgreSQL / SQLite
- **API Logic:** Generic Class-Based Views (CBVs) with automated serialization

## 🏗️ Architecture

The application follows a **Decoupled Headless Architecture**:
1.  **RESTful API:** A stateless backend handling business logic, UUID generation, and data serialization.
2.  **Client-Side:** A Next.js "use client" application that manages global state and interacts with the API via secure interceptors.


## ⚙️ Installation & Setup

### 1. Backend Setup
```bash
cd backend
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install django djangorestframework django-cors-headers
python manage.py migrate
python manage.py runserver
