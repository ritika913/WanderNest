# WanderNest - A Full-Stack Vacation Rental Platform 🌍

## 🚀 Project Overview
This repository contains the source code for Wanderlust, a full-stack web application inspired by Airbnb. It's built with a classic MVC (Model-View-Controller) architecture using Node.js, Express, and MongoDB. The platform allows users to browse, create, and review vacation listings, with features like image uploads, responsive UI, and secure user authentication.

---

## ✨ Core Features

- **RESTful CRUD Operations:** Full Create, Read, Update, and Delete functionality for both listings and reviews.
- **User Authentication:** Secure user signup, login, and logout functionality using Passport.js with password hashing and salting.
- **Image Uploads:** Seamless image uploads to the cloud using Multer for handling multipart/form-data and Cloudinary for hosting.
- **Authorization & Security:** Users can only edit or delete their own listings and reviews.
- **Responsive Design:** Fully responsive user interface built using Bootstrap and EJS templates.
- **Server-Side Validation:** Robust server-side schema validation using Joi to ensure data integrity.
- **Persistent Sessions:** User sessions are stored using connect-mongo, allowing users to stay logged in even after the server restarts.
- **Flash Messaging:** Provides users with feedback (e.g., success or error messages) using connect-flash.
- **MVC Architecture:** Structured backend following MVC design principles for better scalability and maintainability.

image image image image

---

## 🛠 Tech Stack

| Category | Technology |
|----------|------------|
| Backend | Node.js, Express.js |
| Database | MongoDB (with Mongoose ODM), MongoDB Atlas for production |
| Frontend | EJS (Embedded JavaScript templates), Bootstrap 5 |
| Authentication | Passport.js (Local Strategy), Express Session |
| Image Hosting | Cloudinary API, Multer |
| Deployment | Render |

---

## 📂 Repository Structure

<img width="124" height="299" alt="image" src="https://github.com/user-attachments/assets/4ed3bd77-d044-4b15-bf1a-489a6ab62a18" />


---

## 🔧 Local Setup & Installation

Follow these steps to get the project running on your local machine.

### 1. Prerequisites

- Node.js (v18.x or later)
- npm
- A MongoDB Atlas account (or a local MongoDB installation)

---

### 2. Clone the Repository

```bash
git clone https://github.com/your-username/wanderlust.git

cd wanderlust
```

---

### 3. Install Dependencies

```bash
npm install
```

---

### 4. Set Up Environment Variables

Create a `.env` file in the root of the project and add the following variables. Replace the placeholder values with your own credentials.

```env
# MongoDB Atlas Connection String
ATLASDB_URL=mongodb+srv://<username>:<password>@cluster.mongodb.net/wanderlust?retryWrites=true&w=majority

# Cloudinary Credentials
CLOUD_NAME=your_cloud_name
CLOUD_API_KEY=your_api_key
CLOUD_API_SECRET=your_api_secret

# Session Secret Key
SECRET=a_very_long_and_random_string_for_sessions
```

---

### 5. Initialize the Database (Optional)

To populate the database with sample listings, run the initialization script:

```bash
node init/index.js
```

---

### 6. Run the Application

Start the development server using nodemon:

```bash
nodemon app.js
```

The application will be available at:

```bash
http://localhost:8080
```

---
