# 🗳️ Example Voting Application

This project is a multi-service voting app demonstrating a **polyglot microservices architecture**.  
It is composed of several services, each built with a different technology, connected via **Redis** and **PostgreSQL**.

---

## 📐 Architecture

| Service         | Technology | Description                                                                 |
|-----------------|------------|-----------------------------------------------------------------------------|
| **Vote App**    | Python     | Web app (Flask) for casting votes                                           |
| **Redis**       | Redis      | In-memory data store for queueing votes                                     |
| **Worker**      | .NET Core  | Background service that consumes votes from Redis and stores them in Postgres |
| **Database**    | PostgreSQL | Stores voting results                                                       |
| **Result App**  | Node.js    | Web app (Express) displaying real-time voting results                       |

---

## ⚙️ Environment Setup

| Step | Command                                                                                  |
|------|------------------------------------------------------------------------------------------|
| **1. Clone Repository** | `git clone https://github.com/joshua3309/release-example-voting-app.git` <br> `cd release-example-voting-app` |
| **2. Start Services**   | `docker-compose up --build`                                           |
| **3. Access Apps**      | - Voting App (Python): [http://localhost:5000](http://localhost:5000) <br> - Result App (Node.js): [http://localhost:5001](http://localhost:5001) <br> - Redis: `localhost:6379` <br> - Postgres DB: `localhost:5432` |

---

## 📚 Service Guides

| Service         | Guide Link (Editable Placeholder) |
|-----------------|------------------------------------|
| 🐍 **Vote App** (Python) | [Vote App Guide](#) |
| ⚙️ **Worker** (.NET)     | [Worker Guide](#)   |
| 🌐 **Result App** (Node.js) | [Result App Guide](#) |

> Replace `#` with actual guide links.

---

## 🛠️ Technologies Used

| Component   | Technology |
|-------------|------------|
| Frontend Voting | Python (Flask) |
| Frontend Results | Node.js (Express) |
| Queue       | Redis |
| Background Worker | .NET Core |
| Database    | PostgreSQL |
| Orchestration | Docker & Docker Compose |

---

## 🚀 Deployment

| Method | Command |
|--------|---------|
| **Docker Compose** | `docker-compose up --build -d` |

You can deploy this stack to any Docker-compatible platform (local, cloud, Kubernetes).

---

