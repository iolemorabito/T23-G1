# 🎮 Testing Game - Player Registration & Authentication

## 🏆 Task 2-3: Player Registration and Authentication

The application allows students to **register and authenticate** to save their activity history and unlock more advanced game requirements.  

### 📝 **Registration Process**
- Students provide **name, surname, a valid email address, and a password**.
- The system **validates the data** and assigns a **unique player ID**.
- Additional student details, such as **degree program (Bachelor, Master, etc.)**, may also be collected.

### 🔑 **Authentication Process**
- Students log in using their **registered email and password**.
- If the credentials are **valid**, access is granted to:
  - **Game functionalities**
  - **Session history & analytics**

---

## 🚀 Application Deployment

### 📌 **Prerequisites**
- Install **Docker Desktop**  
- Open a **terminal with administrator privileges**

### ⚙️ **Steps to Deploy**
1. **Start the services**:
   ```bash
   docker-compose up
   ```
   - This command **builds the Docker image** and runs the application.

2. **Access the application** from your browser:
   - 🔗 [Registration Page](http://localhost:8080/register)
   - 🔗 [Login Page](http://localhost:8080/login)

3. **Check the database**:
   - Open a terminal and execute:
     ```bash
     docker exec –it g1-t2t3-app-1 bash
     ```
     - This opens an **interactive shell inside the running container**.

   - Connect to MySQL:
     ```bash
     mysql –u root –p STUDENTSREPO
     ```
     - Login with **username:** `root`, **password:** `password`

4. **Manage database tables** using SQL commands:
   ```sql
   SHOW TABLES;
   SELECT * FROM users;
   DROP TABLE users;
   ```

---

## 🔗 Useful Links
- 🐛 **[Docker Documentation](https://docs.docker.com/)**
- 📌 **[MySQL Commands](https://dev.mysql.com/doc/)**
- 🎮 **Game Repository**: [GitHub](https://github.com/Testing-Game-SAD-2023/T23-G1)

---


