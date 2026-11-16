# 🏥 ClinicHub — Clinic Management & Appointment Platform

ClinicHub is a full-stack clinic management platform designed to streamline healthcare operations, including patient management, doctor profiles, appointment scheduling, and clinic administration.

Built using **Next.js, React, TypeScript, Node.js, MongoDB, and Redis**, the project combines a modern frontend with a containerized backend infrastructure to support organized clinic workflows and scalable application development.

---

## 🚀 Features

- **User Authentication:** Login and role-based access management.
- **Patient Management:** Manage and organize patient records.
- **Doctor Management:** Maintain doctor profiles and related information.
- **Appointment Scheduling:** Organize and manage clinic appointments.
- **Dashboard Interface:** Modern and responsive user interface.
- **REST API Integration:** Communication between frontend and backend services.
- **Real-time Communication:** Socket.IO client integration.
- **State Management:** Centralized application state using Redux Toolkit.
- **Form Handling:** Form management using React Hook Form.
- **Containerized Environment:** Docker-based application and database setup.
- **Caching Infrastructure:** Redis integration in the Docker environment.

---

## 🧱 Tech Stack

| Layer | Technologies |
|---|---|
| Frontend | Next.js 16, React 19, TypeScript |
| Styling | Tailwind CSS 4 |
| State Management | Redux Toolkit, React Redux |
| API Communication | Axios |
| Form Management | React Hook Form |
| Real-time Communication | Socket.IO Client |
| Backend | Node.js, Express |
| Database | MongoDB 7, Mongoose |
| Caching | Redis 7 |
| Development & Deployment | Docker, Docker Compose |
| Monitoring Interface | RedisInsight |

---

## 📦 Project Structure

```text
ClinicHub/
│
├── client/                  # Next.js frontend
│   ├── public/
│   ├── src/
│   ├── package.json
│   └── ...
│
├── server/                  # Backend application
│   ├── ...
│   └── Dockerfile
│
├── .env.docker              # Docker environment variables
├── docker-compose.yml       # Docker services configuration
├── LICENCE
└── README.md
```

---

## 🛠️ Installation & Setup

### Requirements

- Node.js (18 or later)
- npm
- Git
- Docker Desktop
- Docker Compose

### 1. Clone the Repository

```bash
git clone https://github.com/Sahilmore469/ClinicHub.git

cd ClinicHub
```

### 2. Environment Configuration

Configure the environment variables in the `.env.docker` file.

Ensure the required database connection strings, credentials, and backend configuration are properly set.

**Important:** Never commit sensitive environment variables, passwords, or API keys to GitHub.

### 3. Run Using Docker

Build and start all application services:

```bash
docker compose up --build
```

To run in the background:

```bash
docker compose up --build -d
```

### 4. Run Frontend Separately

Navigate to the client directory:

```bash
cd client
```

Install dependencies:

```bash
npm install
```

Start the development server:

```bash
npm run dev
```

Open the application:

http://localhost:3000

### 5. Stop the Application

```bash
docker compose down
```

To remove containers and persistent database volumes:

```bash
docker compose down -v
```

---

## 🐳 Docker Services

| Service | Host Port | Purpose |
|---|---:|---|
| Client | 3000 | Next.js frontend |
| Server | 5000 | Backend API |
| MongoDB | 27018 | Database |
| Redis | 6380 | Caching |
| RedisInsight | 5540 | Redis management interface |

Docker Compose manages the application services and persistent storage volumes.

---

## 💻 Available Frontend Commands

| Command | Description |
|---|---|
| `npm install` | Install dependencies |
| `npm run dev` | Start development server |
| `npm run build` | Build production application |
| `npm run start` | Start production server |
| `npm run lint` | Run ESLint |

---

## 🎯 Project Objectives

- Develop a full-stack clinic management application.
- Build responsive interfaces using Next.js and React.
- Implement frontend and backend communication.
- Manage application state using Redux Toolkit.
- Integrate database and caching infrastructure.
- Use Docker to simplify application setup and development.
- Practice scalable application architecture and full-stack development.

---

## 👨‍💻 Author

**Sahil More**

GitHub: [@Sahilmore469](https://github.com/Sahilmore469)

Project: [ClinicHub](https://github.com/Sahilmore469/ClinicHub)

---

⭐ If you find this project interesting, consider giving it a star!
