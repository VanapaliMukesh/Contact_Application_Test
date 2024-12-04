Contacts Management API (Backend)
Description
This project is the backend implementation for the Contacts Management Application. It provides a robust RESTful API to manage contacts, handle CRUD operations, merge duplicate contacts, validate fields, and secure endpoints through authentication.

Key Features
CRUD Operations:
Endpoints for creating, reading, updating, and deleting contact information.
Supports First Name, Last Name, Email Address, Phone Number, and Address fields.
Contact Merging:
Logic to merge duplicate contacts based on email address or phone number.
Provides an endpoint to trigger merging and resolve duplicates.
Field Validations:
First Name, Last Name (required, alphabetic characters only).
Email (must be unique and in a valid format).
Phone Number (must be unique and in a valid format).
Address (optional, validated if provided).
Authentication:
Secured using JWT (JSON Web Token).
Role-based access control: Admin and Regular User.
Technologies Used
Framework: Express.js (Node.js)
Database: MongoDB (NoSQL)
Authentication: JWT (JSON Web Token)
ORM/ODM: Mongoose for MongoDB schema and validation
Setup Instructions
Prerequisites
.Node.js (>= 14.x)
.MongoDB (local or cloud instance, e.g., MongoDB Atlas)

nstallation Steps
Clone the repository:

bash
Copy code
git clone https://github.com/VanapaliMukesh/Contact_Application_backend.git
cd Contact_Application_backend
Install dependencies:

bash
Copy code
npm install
Create a .env file in the root of the project and add the following environment variables:

bash
Copy code
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
Start the application:

bash
Copy code
npm start
The backend API will be running on http://localhost:5000.

API Documentation
GET /contacts: Get a list of all contacts.
POST /contacts: Create a new contact.
PUT /contacts/:id: Update an existing contact.
DELETE /contacts/:id: Delete a contact.
POST /merge: Merge duplicate contacts based on email or phone number.
For detailed API documentation and testing, use Postman or Swagger (if integrated)
