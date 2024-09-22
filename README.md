<<<<<<< HEAD
# ticket-management-system
=======
# Ticket Management System

A simple RESTful API built with Node.js and MongoDB for managing support tickets.

## Features:
- Create, Read, Update, Delete (CRUD) support tickets.
- Validation and error handling.
- MongoDB for data storage.

## Setup Instructions

### Prerequisites:
- [Node.js](https://nodejs.org/)
- [MongoDB](https://www.mongodb.com/try/download/community)


### Steps to Run the Project:

1. Clone the repository:
  
   git clone https://github.com/anjalic1902/ticket-management-system.git
   cd ticket-management-system

2. Install dependencies:

   npm install

3. Start MongoDB

4. Create a .env file in the project root with the following content:

   MONGO_URI=mongodb://localhost:27017/ticket-system
   PORT=5000

5. Run the application:

   npm start

6. The server should now be running on http://localhost:5000.

### API Documentation

1. Create a New Ticket

   Method: POST /api/tickets
   Body (JSON):


{
    "title": "System Crash on File Upload",
    "description": "The system crashes when a user tries to upload files larger than 50MB.",
    "status": "open"
  }

2. Retrieve All Tickets
   Method: GET /api/tickets
Response:
[
  {
    "title": "System Crash on File Upload",
    "description": "The system crashes when a user tries to upload files larger than 50MB.",
    "status": "open",
    "_id": "66efa86d6e97a3de4773fe57",
    "createdAt": "2024-09-22T05:17:33.045Z",
    "updatedAt": "2024-09-22T05:17:33.045Z",
    "__v": 0
}
]

3. Retrieve a Single Ticket by ID
   Method: GET /api/tickets/:id

4. Update a Ticket
   Method: PUT /api/tickets/:id
   Body (JSON):
{
  "title": "Updated title",
  "description": "Updated description",
  "status": "closed"
}

5. Delete a Ticket
   Method: DELETE /api/tickets/:id
>>>>>>> 20c9f1a (Your commit message here)
