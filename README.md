# Golang REST API

This is a simple REST API built with Golang and Gorilla Mux.

## Endpoints

### Get All Tasks

- **URL:** `/tasks`
- **Method:** `GET`
- **Description:** Retrieves all tasks.
- **Response:**
  ```json
  [
    {
      "ID": 1,
      "Name": "Task One",
      "Content": "Some Content"
    }
  ]

### Get a Single Task

- **URL:** `/tasks/{id}`
- **Method:** `GET`
- **Description:** Retrieves a single task by ID.
- **Response:**
  ```json
    {
    "ID": 1,
    "Name": "Task One",
    "Content": "Some Content"
    }

### Create a Task

- **URL:** `/tasks/`
- **Method:** `POST`
- **Description:** Creates a new task.
- **Request Body:**
  ```json
    {
    "Name": "Task Two",
    "Content": "Some Content 2"
    }
- **Response:**
  ```json
    {
    "ID": 2,
    "Name": "Task Two",
    "Content": "Some Content 2"
    }

### Update a Task

- **URL:** `/tasks/{id}`
- **Method:** `PUT`
- **Description:** Updates an existing task by ID.
- **Request Body:**
  ```json
    {
    "Name": "Updated Task",
    "Content": "Updated Content"
    }
- **Response:**
  ```json
    {
    "ID": 1,
    "Name": "Updated Task",
    "Content": "Updated Content"
    }

### Delete a Task

- **URL:** `/tasks/{id}`
- **Method:** `DELETE`
- **Description:** Deletes a task by ID.
- **Request Body:**
- **Response:**
    The task with ID {id} has been removed successfully

### Running the API
To run the API, use the following command:

The API will be available at http://localhost:3000.

### Postman Collection
You can use the provided Postman collection to test the API. Import the golang-rest-simple.postman_collection.json file into Postman.