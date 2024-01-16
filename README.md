# Task Application

This is a simple task application with the following RESTful API endpoints:

## Get All Tasks

### Endpoint

`GET /tasks`

### Description

Retrieves all tasks.

### Response

A JSON array containing all tasks.

---

## Create a Task

### Endpoint

`POST /tasks`

### Description

Creates a new task.

### Request Body

A JSON object containing the task details.

```json
{
  "title": "Title 1",
  "description": "Description 1"
}
```

### Response

The newly created task as a JSON object.

---

## Update a Task

### Endpoint

`PUT /tasks/{id}`

### Description

Updates a specific task by its ID.

### Parameters

-  `id`: The ID of the task to update.

### Request Body

A JSON object containing the updated task details.

```json
{
  "title": "Title 1",
  "description": "Description 1"
}
```

### Response

The updated task as a JSON object.

---

## Delete a Task

### Endpoint

`DELETE /tasks/{id}`

### Description

Deletes a specific task by its ID.

### Parameters

-  `id`: The ID of the task to delete.

### Response

A success message indicating the task has been deleted.

---

## Complete a Task

### Endpoint

`PATCH /tasks/{id}`

### Description

Marks a specific task as completed.

### Parameters

-  `id`: The ID of the task to complete.

### Response

The updated task with the completion status as a JSON object.