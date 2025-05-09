# lost-and-found-system-backend

Lost & Found System Backend

Overview

This project implements a backend for a campus Lost & Found system using Node.js, Express, and MongoDB. It allows security staff or students to log found items and users to view, update, and manage those entries.

Features

- Create, Read, Update, and Delete (CRUD) operations for lost and found items
- View all unclaimed items
- View one item by ID
- Update item details or mark as claimed
- Delete old or irrelevant entries

Technologies Used

- Node.js
- Express.js
- MongoDB

API Endpoints

- POST /item: Create a new lost and found item
- GET /items: View all unclaimed items
- GET /items/:id: View one item by ID
- *PATCH /items/:id*: Update an item's details or mark as claimed
- *DELETE /items/:id*: Delete an item

Installation and Setup

1. Clone the repository
2. Run `npm install` to install dependencies
3. Set up a MongoDB database and update the connection string in `app.js`
4. Run `npm start` to start the server

Item Model

- `itemName`: String (required)
- `description`: String
- `locationFound`: String (required)
- `dateFound`: Date (required)
- `claimed`: Boolean (default: false)

Future Development

- Implement user authentication and authorization
- Add search functionality
- Integrate with frontend application
