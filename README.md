<h1 align="center">
    ATTENDANCE MANAGEMENT SYSTEM
</h1>

<h3 align="center">
Streamline attendance tracking, organize classes, and manage student and faculty data.<br>
Seamlessly monitor presence, assess student performance, and manage records in one place. <br>
Effortless access to attendance logs, performance insights, and communication tools.
</h3>

<br>
🔗 [Live Website](https://attendance-management-system-8jff4ccev.vercel.app/)
<br><br>
👤 Developed by [Shantanu Kulkarni]

# 🚀 About

The **Attendance Management System** is a full-stack web application built using the **MERN stack** (MongoDB, Express.js, React.js, Node.js). This system helps administrators, teachers, and students keep track of attendance records, student data, and more.

It simplifies and automates the process of marking, recording, and analyzing attendance across classrooms or departments.

## ✨ Features

- **Role-based Access:**
  - Admin, Teacher, and Student roles with specific dashboards and privileges.

- **Admin Dashboard:**
  - Add/remove students and teachers.
  - Create and assign classes.
  - Manage attendance and user credentials.

- **Teacher Dashboard:**
  - Mark daily attendance for classes.
  - Add/view student performance.
  - View attendance history.

- **Student Dashboard:**
  - View attendance status.
  - Track academic progress.
  - Receive teacher feedback.

- **Attendance Reporting:**
  - Generate detailed attendance logs.
  - Filter by date, student, or class.

- **User-Friendly Interface:**
  - Clean and responsive UI with real-time updates.
  - Optimized for both desktop and mobile devices.

## 🛠️ Tech Stack

- **Frontend:** React.js, Redux, Material UI
- **Backend:** Node.js, Express.js
- **Database:** MongoDB (Atlas or Local)
- **Other Tools:** Vercel (Deployment), Render (Backend Hosting)

## 🖥️ Live Demo

🌐 Visit the live app here:  
[https://attendance-management-system-8jff4ccev.vercel.app/](https://attendance-management-system-8jff4ccev.vercel.app/)

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/your-username/attendance-management-system.git
````

### 2. Setup Backend

```bash
cd backend
npm install
```

Create a `.env` file inside the `backend` folder and add:

```
MONGO_URL = your_mongodb_connection_string
```

Start backend:

```bash
npm start
```

### 3. Setup Frontend

```bash
cd frontend
npm install
npm start
```

Now open `http://localhost:3000` in your browser. The backend should run on `http://localhost:5000`.

## 🧪 Error Troubleshooting

### Frontend not loading?

* Check `.env` file in `frontend` folder.
* If API base URL is not working via `.env`, use this fix:

Inside files like `userHandle.js`, `teacherHandle.js`, etc., replace:

```js
process.env.REACT_APP_BASE_URL
```

with:

```js
const REACT_APP_BASE_URL = "http://localhost:5000";
```

And use `REACT_APP_BASE_URL` directly in your API requests.

### Delete not working on deployed site?

For guest/demo purposes, the delete functionality might be disabled.

To enable:

1. Uncomment the original `deleteUser` function in `userHandle.js`.
2. Comment out the version that shows the "delete disabled" message.
3. Do the same in all `Show*.js` files by enabling actual `deleteHandler` logic.

## 🌍 Deployment

* **Frontend:** Vercel
* **Backend:** Render

You can deploy your own version using these platforms with proper `.env` configuration for environment variables.

---

🟢 If you found this project useful, feel free to give it a ⭐ on GitHub and connect with me!
