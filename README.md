# 🏺 Legacy Vault — Server

A RESTful backend service powering the Historical Artifacts Tracker application. This server handles artifact management, user authentication, authorization, database operations, user interactions, and historical data processing.

Built with **Node.js, Express.js, and MongoDB**, the backend provides the core functionality required to support an interactive, data-driven historical artifact platform.

---

## 🌐 Project Information

- **Project:** Legacy Vault
- **Repository:** Server-Side Application
- **Backend Runtime:** Node.js
- **Framework:** Express.js
- **Database:** MongoDB Atlas
- **Deployment Platform:** render

---

## 📖 Overview

The Historical Artifacts Tracker backend is responsible for managing the application's data and business logic.

It provides API functionality for exploring historical artifacts, managing user contributions, handling likes and dislikes, processing comments, managing artifact comparisons, and generating dynamic quizzes from available artifact data.

The backend also integrates authentication and authorization mechanisms to ensure that protected operations and user-specific resources are accessible only to authorized users.

The primary goal is to provide a structured, secure, and maintainable backend for the Historical Artifacts Tracker frontend application.

---

## ✨ Core Features

### 1. Historical Artifact Management

- Retrieve historical artifacts from the database.
- Retrieve detailed information about individual artifacts.
- Add new historical artifacts.
- Update existing artifact information.
- Delete historical artifacts.
- Retrieve featured artifacts based on like counts.

### 2. Authentication & Authorization

- JWT-based authentication flow.
- Generate JSON Web Tokens for authenticated users.
- Validate JWT tokens for protected operations.
- Protect private API resources.
- Support authenticated requests from the frontend application.

### 3. User-Specific Data Management

- Manage artifacts submitted by individual users.
- Retrieve artifacts associated with a specific user.
- Restrict modification and deletion of artifacts to their authorized owners.
- Support user-specific data retrieval and management.

### 4. Like & Dislike System

- Implement interactive artifact like/dislike functionality.
- Toggle user interaction states.
- Update artifact like counts.
- Synchronize interaction data with MongoDB.
- Retrieve popular artifacts based on engagement.

### 5. Comment Management

- Create comments associated with individual artifacts.
- Retrieve comments for specific artifacts.
- Update existing comments.
- Delete personal comments.
- Maintain user-specific comment management.

### 6. Artifact Comparison System

- Support comparison between two historical artifacts.
- Store user-created comparison notes.
- Retrieve saved comparison notes.
- Update and delete existing comparison notes.

### 7. Dynamic Quiz System

- Generate quiz questions dynamically using available artifact data.
- Provide artifact-related questions for knowledge testing.
- Support data-driven quiz functionality without relying exclusively on manually predefined questions.

### 8. Database Integration

- MongoDB integration for persistent application data.
- Database-driven artifact management.
- Support user-generated content.
- Store and retrieve comments, likes, and comparison information.
- Maintain application data across requests.


---

## 🛠️ Technologies Used

### Backend
- **Node.js** – JavaScript runtime environment.
- **Express.js** – Web framework for building RESTful APIs.
- **MongoDB** – NoSQL database for application data management.

### Authentication & Security
- **Firebase Authentication** – User authentication integration.
- **JSON Web Token (JWT)** – Token-based authentication and authorization.
- **CORS** – Cross-Origin Resource Sharing configuration.
- **Cookie Parser** – Cookie parsing middleware.

### Image Management
- **Cloudinary** – Image uploading, storage, and optimization.

### Development Tools
- **dotenv** – Environment variable management.
- **render** – Backend deployment platform.

---

## 🔐 Authentication & Security

The backend uses a Firebase Authentication and JWT-based authentication flow to support protected application functionality.

The authentication process involves:

1. Users authenticate through the frontend application.
2. The backend generates a JWT token for authenticated users.
3. The token is stored on the client side using the application's configured cookie-based authentication flow.
4. Authenticated requests include the required token.
5. The backend validates the token before allowing access to protected resources.

### Protected Operations

Authentication and authorization are used to protect operations such as:

- Creating historical artifacts.
- Updating personal artifact contributions.
- Deleting personal artifacts.
- Managing user-specific comments.
- Managing comparison notes.
- Accessing protected user-specific resources.

The backend also applies ownership checks to prevent users from modifying or deleting resources belonging to other users.

---

## 🗄️ Database

**Database:** MongoDB Atlas

MongoDB is used to store and manage the application's persistent data.

The backend works with data related to:

- Historical artifacts.
- User contributions.
- Artifact likes and interaction states.
- Artifact comments.
- Comparison notes.
- Quiz-related artifact information.

Database operations support the application's CRUD functionality and dynamic data retrieval.

---

## ⚙️ Getting Started

Follow these instructions to run the backend locally.

### Prerequisites

Make sure you have installed:

- Node.js
- npm
- Git
- A MongoDB database connection

### 1. Clone the Repository

```bash
git clone https://github.com/mdyasin0/artifacts-server-side.git
```

### 2. Navigate to the Project Directory

```bash
cd YOUR_SERVER_PROJECT_DIRECTORY
```

### 3. Install Dependencies

```bash
npm install
```

### 4. Configure Environment Variables

Create a `.env` file in the root directory.

Example configuration:

```env
PORT=
USER=
DB_PASS=
JWT_ACCESS_SECRET=
```



Never commit your `.env` file or expose private credentials in a public repository.

### 5. Start the Server

Use the development command configured in your `package.json`.

For example, if your project uses nodemon:

```bash
npm run dev
```

Alternatively, if a start script is configured:

```bash
npm start
```

The server will start on the configured port.

---

## 🚀 Deployment

The backend is deployed using **Vercel**.

- **Backend Hosting:** render
- **Database Hosting:** MongoDB Atlas
- **Authentication:** Firebase Authentication and JWT integration

Environment variables should be configured securely in the deployment environment rather than committed to the repository.

---

## 🔗 Related Application

**Historical Artifacts Tracker — Live Website**

https://assignment-11-1588b.web.app

---

## 👨‍💻 Developer

**MD Yasin**

Full-Stack Web Developer

- **Email:** mdyasin48902@gmail.com

---

## 🎯 Project Objective

This backend project demonstrates practical experience in developing RESTful APIs, integrating databases, implementing authentication and authorization, managing user-generated content, and building data-driven application functionality.

It represents hands-on work with Node.js, Express.js, MongoDB, JWT, Firebase Authentication in the development of a full-stack web application.

---

**Developed as part of the Legacy Vault project.**
