# Contact Application Backend

This is the **backend** of the **Contact Application**, which is built using **Node.js** and **Express**. The backend handles all the server-side logic, including managing contacts, handling requests, and connecting to the database.

## Features

- **API Endpoints**: Provides various API routes to handle CRUD operations for contacts (Create, Read, Update, Delete).
- **Database Integration**: Connects to a database (e.g., MongoDB) to store and retrieve contact information.
- **Authentication (Optional)**: Secures endpoints with authentication mechanisms such as JWT (if implemented).
  
## Tech Stack

- **Node.js**: Server-side JavaScript runtime.
- **Express**: Web framework for building RESTful APIs.
- **MongoDB** (or any database of choice): NoSQL database for storing contact information.
- **Mongoose** (if using MongoDB): ODM (Object Data Modeling) for MongoDB.
- **Cors**: Middleware to enable cross-origin requests from the frontend.
- **dotenv**: Loads environment variables for configuration.

## Installation

### Clone the Repository

Clone the repository to your local machine:

```bash
git clone https://github.com/VanapaliMukesh/Contact_Application_Test.git
cd Contact_Application_Test

Navigate to the backend directory:

bash
Copy code
cd server
Install the required dependencies:

bash
Copy code
npm install
Configuration
Create a .env file in the root of the backend directory.

Add the following environment variables to the .env file:

plaintext
Copy code
PORT=5000
MONGO_URI=<your-mongo-db-uri>
JWT_SECRET=<your-jwt-secret>
Replace <your-mongo-db-uri> with your MongoDB connection string (or any database URI you're using) and <your-jwt-secret> with a secret key if using authentication.

Running the Server
To start the backend server:

bash
Copy code
npm start
The server will be running on http://localhost:5000.

API Endpoints
GET /api/contacts: Retrieve all contacts.
POST /api/contacts: Add a new contact.
PUT /api/contacts/:id: Update an existing contact.
DELETE /api/contacts/:id: Delete a contact.
You can test the API endpoints using Postman or any other API testing tool.
