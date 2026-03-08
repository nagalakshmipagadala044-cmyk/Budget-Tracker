
# 📝 Budget Tracker Web Application

A Budget Tracker is a tool or application designed to help individuals or businesses manage their finances by tracking income, expenses, and savings. It provides an organized way to monitor financial activity, set spending limits, and plan for future financial goals.

---

## 🌟 Features

- 🔐 **User Authentication (JWT-based)**  
- 🗂️ **Add & Manage Income**
- 🗓️ **Track by Date or Range**
- 📋 **Add, Edit, Delete, and View Expenses**
- ⏰ **Reminders & Browser Notifications (with ringtone)**
- 🎯 **Set Budget Goals**
- 📊 **Live Dashboard with Financial Summary**
- 🌓 **Dark/Light Theme Toggle**
- 💻 **Fully Responsive UI for Mobile, Tablet, and Desktop**

---

## 🧩 Technologies Used

### Frontend
- **HTML5, CSS3, JavaScript**
- **Bootstrap** for responsive design
- **Fetch API** for RESTful API communication
- **Browser Notification API**
- **Custom CSS** for animations and themes

### Backend
- **Node.js** for runtime environment
- **Express.js** for RESTful APIs and routing
- **Mongoose** to interact with MongoDB
- **bcryptjs** for secure password hashing
- **jsonwebtoken (JWT)** for authentication

### Database
- **MongoDB** (NoSQL database)
- **Collections:**
  - `users`: Stores registered user information.
  - `scheduled-tasks`: Stores all task data (title, description, priority, due date, status, etc.)

---

## 🛠️ Installation & Setup
### 1. Install Dependencies (Backend)
```bash
npm install
```

### 2. MongoDB Setup
- Make sure MongoDB is installed and running.
- Default connection: `mongodb://localhost:27017/budget-tracker`

### 3. Run the Server
```bash
node server.js
```

### 4. Open the App
- Open `index.html` in your browser to start using the app.

---

## 🧪 Project Structure

```
project-root/
├── index.html             # Splash screen + Sidebar navigation
├── budget-tips.html       # Tips to save our budget
├── dashboard.html         # Task dashboard and expense list
├── summary.html           # Summary page
├── login.html             # Login page
├── register.html          # Register page
├── server.js              # Node.js Express backend server
├── style.css              # Global styles
├── assets/                # Logo and icons
└── README.md              # Project documentation
```

---

## 🔐 Security Highlights

- All passwords are hashed before storing in MongoDB using **bcryptjs**.
- Sessions are managed securely using **JWT tokens** stored on the client side.
- Input validation prevents XSS attacks and SQL/NoSQL injection.
- Token expiry is handled to enforce session logout after a defined period.

---

## 🌍 Future Enhancements

- 🔔 Custom Alerts & Notifications
- 🔁 Recurring Transactions
- 🔒 Two-Factor Authentication (2FA)
- 📆 Budget History & Trends Over Time
- 🎯 Goal-Based Saving Planner
