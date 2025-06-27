---

## 📘 `README.md`

# Student-CRUD-App

This is a simple RESTful API built with **Node.js**, **Express**, and **MongoDB** for managing student records.  
It supports full CRUD operations (Create, Read, Update, Delete) and includes validation and error handling.

---

## 📦 Tech Stack

- **Node.js**
- **Express**
- **MongoDB** (Mongoose)
- **Postman** (for testing)
- **Nodemon** (dev server)

---

## 📁 Project Structure



student-api/
│
├── src/
│   ├── config/              # MongoDB connection
│   │   └── db.js
│   ├── controller/          # Logic for endpoints
│   │   └── student.controller.js
│   ├── models/              # Student schema
│   │   └── student.schema.js
│   ├── routes/              # Express router
│   │   └── studentRoutes.js
│   └── student.js           # Main entry point
│
├── .env
├── package.json
└── README.md

````

---

## 🚀 How to Run

### 1. Clone the Repo

```bash
git clone https://github.com/Ray-456/Student-CRUD-App.git
cd Student-CRUD-App
````

### 2. Install Dependencies

```bash
npm install
```

### 3. Set Up Environment

Create a `.env` file in the root:

```env
PORT=3000
MONGODB_URI=mongodb://localhost:27017/studentsDB
```

### 4. Start Server

```bash
npm run dev
```

---

## 🔌 API Endpoints

| Method | Endpoint          | Description             |
| ------ | ----------------- | ----------------------- |
| POST   | `/students`       | Create a new student    |
| GET    | `/students`       | Get all students        |
| GET    | `/students/count` | Get total student count |
| PUT    | `/students/:id`   | Update student by ID    |
| DELETE | `/students/:id`   | Delete student by ID    |

---

## ⚠️ Error Handling

* `400 Bad Request`: Invalid or missing fields
* `404 Not Found`: Student not found
* `409 Conflict`: Email already exists

---

## 🧪 Postman Collection

1. Import `postman_collection.json` into Postman.
2. Hit the endpoints with sample data.
3. Tests for status codes and response structures included.

---

## 📝 Notes

* Emails must be unique — enforced via Mongoose index.
* All fields are required: `firstName`, `lastName`, `email`, `age`.
* Data stored in MongoDB under `studentsDB` database.

---

## 💡 Bonus Features (Optional)

✅ Not implemented yet — but planned:

* Pagination: `/students?page=1&limit=10`
* Filtering: `/students?lastName=Smith`

---

## 📞 Questions?

Raise an issue or [ping me on GitHub](https://github.com/Ray-456) 💬

```

---

Copy that into your `README.md` file, commit it, push to GitHub.

Want me to generate the Postman collection next? Or you wanna flex and do it yourself?
```
