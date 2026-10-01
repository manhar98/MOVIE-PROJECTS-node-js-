# 🎬 Movie API

A RESTful **Movie API** built using **Node.js, Express.js, and MongoDB**.

This project provides complete **CRUD (Create, Read, Update, Delete)** operations for managing movie information. The project follows the **MVC (Model-View-Controller) architecture** and APIs are tested using **Postman**.

---

## 📌 Project Information

### Project Name
**Movie API**

### Project Type
RESTful API / Backend Project

### Description

The Movie API allows users to manage movie data through RESTful APIs.

The project supports:

- Create a new movie
- Get all movies
- Get a single movie by ID
- Update movie details
- Delete a movie

The project uses MongoDB as the database and Mongoose for database interaction.

---

## 🛠️ Technologies

- **Node.js** – JavaScript runtime environment
- **Express.js** – Backend web framework
- **MongoDB** – NoSQL database
- **Mongoose** – MongoDB object modeling library
- **CORS** – Cross-Origin Resource Sharing
- **dotenv** – Environment variable management
- **Nodemon** – Automatically restarts the server during development
- **Postman** – API testing
- **MongoDB Compass** – Database management and monitoring

---

## 📂 Folder Structure

```text
movie-api/
│
├── src/
│   ├── controllers/
│   │   └── movieControllers.js
│   │
│   ├── db/
│   │   └── db.js
│   │
│   ├── middleware/
│   │
│   ├── models/
│   │   └── movieModel.js
│   │
│   └── routes/
│       └── movieRoutes.js
│
├── .env
├── .gitignore
├── package.json
├── package-lock.json
├── server.js
└── README.md
```

---

## 🏗️ MVC Architecture

This project follows the **MVC architecture**.

### Model
The `movieModel.js` file defines the Movie schema and structure.

Movie fields include:

- Title
- Director
- Genre
- Release Year
- Rating
- Description

### Controller
The `movieControllers.js` file contains the main CRUD logic.

It handles:

- Creating movies
- Getting movies
- Getting a movie by ID
- Updating movies
- Deleting movies

### Routes
The `movieRoutes.js` file defines the API endpoints and connects them with the appropriate controller functions.

### Database
The `db.js` file is responsible for connecting the application with MongoDB using Mongoose.

---

## ⚙️ Installation / Setup

### 1. Clone the Repository

```bash
git clone https://github.com/manhar98/MOVIE-PROJECTS-node-js-.git
```

### 2. Go to the Project Folder

```bash
cd node_pr5-movie
```

### 3. Install Dependencies

```bash
npm install
```

### 4. Create `.env` File

Create a `.env` file in the project root:

```env
PORT=5000
MONGO_URI=mongodb://127.0.0.1:27017/movieDB
```

You can use your own MongoDB connection string if required.

### 5. Start the Development Server

```bash
npm run dev
```

The server will run on:

```text
http://localhost:5000
```

### 6. Check the API

Open:

```text
http://localhost:5000
```

Expected response:

```json
{
  "message": "Movie API is running successfully"
}
```

---

## 🔗 API Endpoints

Base URL:

```text
http://localhost:5000/api/movies
```

| Method | Endpoint | Description |
|---|---|---|
| POST | `/api/movies` | Create a new movie |
| GET | `/api/movies` | Get all movies |
| GET | `/api/movies/:id` | Get movie by ID |
| PUT | `/api/movies/:id` | Update movie |
| DELETE | `/api/movies/:id` | Delete movie |

---

## 🔄 CRUD Details

### 1. Create Movie

**Method:** `POST`

**Endpoint:**
```text
/api/movies
```

**Example Request Body:**

```json
{
  "title": "3 Idiots",
  "director": "Rajkumar Hirani",
  "genre": "Comedy",
  "releaseYear": 2009,
  "rating": 8.4,
  "description": "A story about friendship, college life and dreams."
}
```

This API creates and stores a new movie in MongoDB.

---

### 2. Get All Movies

**Method:** `GET`

**Endpoint:**
```text
/api/movies
```

This API returns all movies stored in the database.

---

### 3. Get Movie By ID

**Method:** `GET`

**Endpoint:**
```text
/api/movies/:id
```

**Example:**
```text
/api/movies/68da123456789
```

This API returns the details of a specific movie using its MongoDB ID.

---

### 4. Update Movie

**Method:** `PUT`

**Endpoint:**
```text
/api/movies/:id
```

**Example Request Body:**

```json
{
  "title": "Interstellar",
  "director": "Christopher Nolan",
  "genre": "Science Fiction",
  "releaseYear": 2014,
  "rating": 8.7,
  "description": "A team of explorers travels through space to find a new home for humanity."
}
```

This API updates an existing movie using its ID.

---

### 5. Delete Movie

**Method:** `DELETE`

**Endpoint:**
```text
/api/movies/:id
```

This API deletes a movie from the MongoDB database using its ID.

---

## 🧪 Postman Testing

All CRUD APIs were tested using **Postman**.

### APIs Tested

- `POST /api/movies` — Add a new movie
- `GET /api/movies` — Get all movies
- `GET /api/movies/:id` — Get a specific movie
- `PUT /api/movies/:id` — Update movie information
- `DELETE /api/movies/:id` — Delete a movie

### Postman Testing Flow

```text
Postman
   ↓
API Route
   ↓
Controller
   ↓
Movie Model
   ↓
MongoDB
```

---

## 🍃 MongoDB Compass

MongoDB Compass is used to:

- View the Movie database
- Check the Movie collection
- Verify inserted movie data
- Check updated movie data
- Verify deleted movie records


---

## 🔗 GitHub Repository

https://github.com/manhar98/MOVIE-PROJECTS-node-js-.git

---

## 👨‍💻 Project Summary

This project demonstrates how to build a RESTful backend API using **Node.js and Express.js** with **MongoDB** as the database.

The project follows MVC architecture and implements complete CRUD functionality for movie management.

### Main Flow

```text
Client / Postman
       ↓
Express Server
       ↓
Routes
       ↓
Controllers
       ↓
Movie Model
       ↓
MongoDB
```

---

## ✅ Project Requirements Completed

- [x] Node.js + Express.js
- [x] Express Server
- [x] Routing
- [x] Middleware
- [x] MVC Architecture
- [x] MongoDB Database
- [x] MongoDB Compass
- [x] Complete CRUD APIs
- [x] Postman API Testing
- [x] GitHub Repository
- [x] Project Documentation
- [x] Project Explanation Video
