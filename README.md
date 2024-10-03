# Event Registration System API

## Overview

This project is a RESTful API designed to power a event registration system. It provides essential CRUD (Create, Read, Update, Delete) operations for managing events. The API interacts with a database (either SQL or NoSQL) to store and retrieve article data, and it includes functionality for handling article creation, retrieval, updating, and deletion.

## Skills and Technologies Used

- **CRUD Operations**: To perform the basic operations such as creating, reading, updating, and deleting events.
- **Databases**: Either SQL (e.g., MySQL, PostgreSQL) or NoSQL (e.g., MongoDB) to store and manage events.
- **RESTful API**: Server-side API that follows REST principles, enabling easy communication between the backend and clients.

## API Endpoints

### 1. **Get a List of Events**

- **Endpoint**: `/events`
- **Method**: `GET`
- **Description**: Returns a list of all published events.

### 2. **Get a Single Event**

- **Endpoint**: `/events/{id}`
- **Method**: `GET`
- **Description**: Returns a specific event identified by its unique ID.

### 3. **Create a New Event**

- **Endpoint**: `/events`
- **Method**: `POST`
- **Description**: Creates a new event with the provided content. The event will be saved in the database and made available for reading.
- **Request Body**:
  - `name`: The name of the event.
  - `description`: The description of the event.
  - `event_date`: Date of the event

### 4. **Update an Event**

- **Endpoint**: `/events/{id}`
- **Method**: `PUT`
- **Description**: Updates an existing event by its ID. The name, description, or event_date of the event can be modified.
- **Request Body**:
  - `name`: The updated event name.
  - `description`: The updated event description.
  - `event_date`: The updated event date

### 5. **Delete an Event**

- **Endpoint**: `/events/{id}`
- **Method**: `DELETE`
- **Description**: Deletes a specific event from the database using its ID.

