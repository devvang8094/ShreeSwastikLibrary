# 📚 ShreeSwastikLibrary — Full Stack Library Management System

A complete **library management system** built for *Shree Swastik Library, Indore* — featuring a responsive frontend, secure admin dashboard, OTP password reset, WhatsApp notifications, and dynamic UI based on student plan expiry.

---

## 🚀 Live Demo

**Frontend:**  
https://devvang8094.github.io/library-website/HTML/home.html  

**Backend API:**  
https://library-backend-production-38a7.up.railway.app/

---

## ✨ Features

### 👤 Student / Visitor View
- Browse library plans (Recliner / Normal seating)  
- View gallery and facilities  
- Contact instantly via WhatsApp  
- Fully mobile responsive (tested on different screen sizes)  
- Clean UI with modern, soft color palette  

---

### 🔐 Admin Features

#### ⭐ Secure Login (Token Based)
- Admin must log in to access dashboard  
- All admin pages are protected  
- Direct URL access to dashboard/management pages is blocked  

#### ⭐ OTP-Based Password Reset
- Admin enters registered email  
- OTP is sent via backend service  
- OTP verification before resetting password  
- Prevents unauthorized access to admin account  

---

### 📝 Student Management

- Add new students with name, phone, plan, and dates  
- Update existing student records  
- Delete students safely  
- Search students by name  
- Sorted by **remaining days** so urgent cases appear first  

#### 🎨 Color-Coded Student Cards
- 🟢 **Green** → More than 5 days left  
- 🟡 **Yellow** → 1–5 days left (expiring soon)  
- 🔴 **Red** → Plan expired  

This visual system helps admin quickly see which students need follow-up.

---

### ☎️ WhatsApp Auto Notification

Each student card has a **Notify** button:

- Opens WhatsApp with a pre-filled message  
- Includes student name and remaining validity  
- Used to send renewal reminders in one click  

---

### 🖥️ Admin Dashboard UI

- Shows **total students** at a glance  
- Quick action cards for:
  - Add Student  
  - View / Manage Students  
- Simple, mobile-friendly layout  
- Focused on clarity and productivity  

---

## 🛠️ Tech Stack

### Frontend
- **HTML5**  
- **CSS3**  
- **JavaScript (Vanilla JS)**  
- Responsive layout using flexbox and media queries  

### Backend
- **Node.js**  
- **Express.js**  
- **JSON Web Tokens (JWT)** or custom token logic for auth  
- **Nodemailer** (for OTP email sending)  

### Database
- **MySQL** (hosted on Railway/Aiven)  

---

## 📂 Project Structure

```bash
ShreeSwastikLibrary/
│
├── frontend/
│   ├── HTML/
│   │   ├── home.html
│   │   ├── admin-dashboard.html
│   │   ├── add-student.html
│   │   ├── manage-students.html
│   │   ├── view-students.html
│   │   ├── update-students.html
│   │   └── forgot-password.html
│   │
│   ├── CSS/
│   │   ├── homeStyle.css
│   │   ├── admin-dashboard.css
│   │   ├── add-student.css
│   │   ├── manage-students.css
│   │   ├── view-students.css
│   │   ├── update-students.css
│   │   └── admin-login.css
│   │
│   ├── JS/
│   │   ├── home.js
│   │   ├── admin-dashboard.js
│   │   ├── add-student.js
│   │   ├── manage-students.js
│   │   ├── view-students.js
│   │   ├── update-students.js
│   │   ├── admin-login.js
│   │   └── forgot-password.js
│   │
│   ├── Images/
│   │   ├── icons, gallery images, logo, etc.
│   │   └── will-look-like/ (UI preview screenshots)
│   │
│   └── index.html
│
└── backend/
    ├── src/ 
    ├── index.js                # Main server file
    ├── routes/                 # Express routes
    ├── controllers/            # Controllers / handlers
    ├── utils/                  # Helper functions (if any)
    ├── package.json
    ├── package-lock.json
    ├── .gitignore              # Ignores .env and node_modules
    └── (Environment variables stored in local .env, NOT committed)
---

## 🚧 Future Improvements

- Add role-based access (multiple admins)  
- Add analytics (daily active students, renewals, etc.)  
- Export student data to Excel/CSV  
- Add payment integration for online renewals  
- Dark mode for dashboard  

---

## 👨‍💻 Author

**Deepak Patidar**  
Full Stack Developer – JavaScript | Node.js | MySQL  

Feel free to open issues or suggestions if you have ideas to improve this project!

