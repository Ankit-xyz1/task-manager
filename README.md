deployed here : https://task-manager-two-xi.vercel.app/


# Task Manager API

This is a simple Task Manager API built with Node.js and Express. It allows users to create, fetch, update, and delete tasks.

## Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/your-username/task-manager.git
   ```
2. Navigate to the project directory:
   ```sh
   cd task-manager
   ```
3. Install dependencies:
   ```sh
   npm install
   ```

## Running the Server

To start the server, run:

```sh
npm start
```

The server will run on `http://localhost:3000` (default port).

## API Endpoints

### 1. Get All Tasks
   - **Endpoint:** `GET /api/tasks`
   - **Description:** Fetches all tasks.
   - **Response Example:**
     ```json
     [
       {
         "id": "1",
         "title": "Complete project",
         "status": "pending"
       },
       {
         "id": "2",
         "title": "Buy groceries",
         "status": "completed"
       }
     ]
     ```

### 2. Create a Task
   - **Endpoint:** `POST /api/tasks`
   - **Description:** Creates a new task.
   - **Request Body:**
     ```json
     {
       "title": "New Task",
       "status": "pending"
     }
     ```
   - **Response Example:**
     ```json
     {
       "id": "3",
       "title": "New Task",
       "status": "pending"
     }
     ```

### 3. Update a Task
   - **Endpoint:** `PUT /api/tasks/:id`
   - **Description:** Updates an existing task by ID.
   - **Request Body Example:**
     ```json
     {
       "title": "Updated Task",
       "status": "completed"
     }
     ```
   - **Response Example:**
     ```json
     {
       "id": "3",
       "title": "Updated Task",
       "status": "completed"
     }
     ```

### 4. Delete a Task
   - **Endpoint:** `DELETE /api/tasks/:id`
   - **Description:** Deletes a task by ID.
   - **Response Example:**
     ```json
     {
       "message": "Task deleted successfully"
     }
     ```

## Technologies Used
- Node.js
- Express.js

## Contributing
Feel free to submit issues and pull requests.

## License
This project is licensed under the MIT License.

