# Student Management System using MERN Stack

This is a full-stack Student Management System built with the MERN stack (MongoDB, Express.js, React.js, and Node.js). The application allows users to **create**, **read**, **update**, and **delete (CRUD)** student records. Each record contains the student's **Name, Registration Number, Phone Number, Age, and Department**.

## 🚀 Features

- Add new student records
- View all students in a clean table layout
- Edit existing student information
- Delete student records
- Responsive and clean UI using React

## 📌 Tech Stack

- **Frontend**: React.js, Axios, CSS
- **Backend**: Node.js, Express.js
- **Database**: MongoDB (via Mongoose)
- **Environment**: `.env` file used in backend for secure config

## 🔧 Installation

### 1. Clone the Repository

```bash
git clone https://github.com/Yadhavaramanan/Student-Management-System-using-MERN-Stack.git
cd Student-Management-System-using-MERN-Stack
```

### 2.Setup Backend
```
cd backend
npm install
```
Create a .env file inside the backend folder:

```
PORT=5000
MONGODB_URI=your_mongodb_connection_string_here
```

Then start the backend:
```
npm start 
```

### 3. Setup Frontend
In a terminal:
```
cd frontend
npm install
npm start
```
---

## 📂 Folder Structure

```
Student-Management-System/
│
├── backend/
│   ├── models/
│   ├── routes/
│   ├── .env
│   └── server.js
│
├── frontend/
│   ├── public/
│   ├── src/
│   └── App.js
│
└── README.md
```
---
## 🤝 Author

Yadhavaramanan C
GitHub: @Yadhavaramanan

---
## 📄 License

This is a personal project for learning and understanding the CRUD Operations.

---



Nice 🔥 — since you’re using **AWS EC2**, I’ll give you **exact step-by-step commands (copy-paste ready)** to:

✔ Clone your repo
✔ Setup backend
✔ Run server
✔ (Optional) Setup frontend
✔ Make it publicly accessible

---

# ☁️ 1. Connect to EC2

From your local terminal:

```bash
ssh -i your-key.pem ubuntu@your-ec2-public-ip
```

---

# 📦 2. Update System

```bash
sudo apt update && sudo apt upgrade -y
```

---

# 🟢 3. Install Node.js & npm

```bash
curl -fsSL https://deb.nodesource.com/setup_18.x | sudo -E bash -
sudo apt install -y nodejs
```

Check:

```bash
node -v
npm -v
```

---

# 📥 4. Clone Your GitHub Repo

```bash
git clone https://github.com/kaustubhgharat/Student_Record_Management.git
cd Student_Record_Management
```

---

# 📂 5. Install Dependencies

(Inside project folder)

```bash
npm install
```

---

# 🔐 6. Setup Environment Variables

Create `.env` file:

```bash
nano .env
```

Add (example):

```
PORT=5000
MONGO_URI=your_mongodb_atlas_connection_string
```

Save:

* `CTRL + X`
* `Y`
* `Enter`

---

# ▶️ 7. Run Backend Server

```bash
node server.js
```

OR (if using nodemon):

```bash
npx nodemon server.js
```

---

# 🌐 8. Allow Port in AWS (IMPORTANT)

Go to EC2 → Security Groups → Edit Inbound Rules

Add:

| Type       | Port | Source    |
| ---------- | ---- | --------- |
| Custom TCP | 5000 | 0.0.0.0/0 |

---

# 🌍 9. Test in Browser

Open:

```
http://your-ec2-public-ip:5000
```

---

# ⚡ 10. Run in Background (PM2 - Recommended)

Install PM2:

```bash
sudo npm install -g pm2
```

Start app:

```bash
pm2 start server.js
```

Save process:

```bash
pm2 save
pm2 startup
```

---

# 🖥️ 11. (Optional) Frontend Setup

If your repo has frontend folder:

```bash
cd frontend
npm install
npm run build
```

Install serve:

```bash
sudo npm install -g serve
serve -s build
```

---

# 🌐 12. Open Frontend Port

Allow port **3000 or 5000** in AWS security group.

---

# 🔥 Final Output

You’ll have:

* Backend running on:

  ```
  http://<EC2-IP>:5000
  ```
* Frontend (if deployed):

  ```
  http://<EC2-IP>:3000
  ```

---

# 💡 Bonus (Better Production Setup)

If you want full marks 💯, add:

### Use NGINX (optional but impressive)

```bash
sudo apt install nginx -y
```

---

# 🚨 Common Errors

| Issue                | Fix                  |
| -------------------- | -------------------- |
| App not opening      | Check security group |
| Mongo not connecting | Check MONGO_URI      |
| Port already used    | Change PORT          |

---

# ✅ If you want next

I can help you with:

✔ NGINX setup (domain + reverse proxy)
✔ Docker deployment (very important for CC)
✔ Fix errors from your repo specifically
✔ Complete report + architecture diagram

Just tell me 👍

