# 🐾 Pet Care Organizer — Backend REST API

A full-featured backend application for managing pet care operations, built with Java and Spring Boot. Supports user authentication, pet records, appointment scheduling, and health tracking through a RESTful API.

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Language | Java 17 |
| Framework | Spring Boot, Spring MVC, Spring Data JPA |
| Database | MySQL |
| Containerization | Docker, Docker Compose |
| Testing | JUnit |
| Version Control | Git / GitHub |

---

## ✨ Features

- **User Authentication** — Register and manage user accounts
- **Pet Records** — Create, update, and delete pet profiles
- **Appointment Scheduling** — Book and manage vet appointments
- **Health Tracking** — Log and retrieve pet health history
- **Reminders** — Set care reminders for pets
- **12+ REST API Endpoints** — Full CRUD operations via JSON

---

## 🏗️ Architecture

Follows **Controller → Service → Repository** layered architecture:

```
src/
├── controller/    # REST API endpoints
├── service/       # Business logic
├── repository/    # Database access (JPA)
├── model/         # Entity classes
└── dto/           # Data transfer objects
```

## 🚀 Running Locally

### With Docker (Recommended)

```bash
# Clone the repo
git clone https://github.com/JankiPatel349/Petcare-backend.git
cd Petcare-backend

# Start app and database
docker-compose up --build
```

API will be available at `http://localhost:8080`

### Without Docker

1. Install Java 17+ and MySQL
2. Create a database named `petcare`
3. Update `src/main/resources/application.properties` with your DB credentials
4. Run: `./mvnw spring-boot:run`

---

## 📡 API Endpoints (Sample)

| Method | Endpoint | Description |
|---|---|---|
| POST | `/api/users/register` | Register new user |
| POST | `/api/users/login` | User login |
| GET | `/api/pets` | Get all pets for user |
| POST | `/api/pets` | Add new pet |
| PUT | `/api/pets/{id}` | Update pet record |
| DELETE | `/api/pets/{id}` | Delete pet |
| GET | `/api/appointments` | Get appointments |
| POST | `/api/appointments` | Schedule appointment |

---

## 👩‍💻 Author

**Janki Patel**  
[LinkedIn](https://linkedin.com/in/janki-patel-262315329) • [GitHub](https://github.com/JankiPatel349)
