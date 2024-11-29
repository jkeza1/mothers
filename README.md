# mothers



# Smeef Project
Smeef is a platform empowering single mothers through skill-building, career opportunities, and entrepreneurial guidance. This repository contains the source code for the Smeef platform.

#Table of Contents
Features
Technologies Used
Prerequisites
Installation
Setup and Configuration
Running the Project
Deployment
Contributing
License
Features
User roles: Admin, Mentor, and Single Mother.
Dashboard with tailored content based on user roles.
Course management for single mothers.
Job board for career opportunities.
Secure authentication and authorization.
Responsive design using TailwindCSS.
Technologies Used
Backend: Node.js, Express.js, Mongoose
Frontend: HTML, TailwindCSS, JavaScript
Database: MongoDB (MongoDB Atlas)
Deployment: Render
Prerequisites
Ensure you have the following installed on your system:

Node.js (v18 or higher)
npm (Node Package Manager)
Git
MongoDB Atlas Account (or a locally running MongoDB instance)
An IDE or Text Editor (e.g., VSCode)
Installation
Step 1: Clone the Repository
bash
Copy code
git clone https://github.com/jkeza1/mothers.git
cd mothers
Setup and Configuration
Step 2: Install Dependencies
Navigate to the project directory and install the required packages:

bash
Copy code
npm install
Step 3: Configure the .env File
Create a .env file in the root directory and add the following configuration. Replace placeholders with actual values:

env
Copy code
PORT=3005
MONGO_URI=mongodb+srv://<your_username>:<your_password>@cluster0.abkhk.mongodb.net/<your_database_name>?retryWrites=true&w=majority
Step 4: Set Up MongoDB
Log in to your MongoDB Atlas account.
Create a cluster and whitelist your IP address.
Replace the <your_username>, <your_password>, and <your_database_name> placeholders in the MONGO_URI with your actual credentials.
Running the Project
Step 5: Start the Server
Run the development server:

bash
Copy code
npm run dev
The app will start at http://localhost:3005.

Project Structure
csharp
Copy code
mothers/
│
├── src/
│   ├── app.js          # Main server file
│   ├── routes/         # API routes
│   ├── models/         # Mongoose schemas
│
├── public/             # Frontend HTML, CSS, and JS files
├── templates/          # HTML templates for pages
├── .env                # Environment variables (not included in Git)
├── README.md           # Documentation
├── package.json        # Project metadata
└── package-lock.json   # Exact dependency tree
Deployment
This project is deployed on Render. Follow these steps to deploy:

Create an account on Render.
Create a new Web Service.
Connect your GitHub repository to Render.
Add the following environment variables in the Render dashboard:
PORT
MONGO_URI
Deploy the service and obtain the public URL.
