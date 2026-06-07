# Task Management API Documentation

## Overview

This API enables applications to create, retrieve, update, and delete tasks.

## Base URL

https://api.example.com/v1

## Authentication

Bearer Token Authentication

Authorization: Bearer <token>

## Get Tasks

### Request

GET /tasks

### Response

{
"id": 1001,
"title": "Review Documentation",
"status": "Open"
}

## Create Task

### Request

POST /tasks

{
"title": "Create User Guide",
"priority": "High"
}

### Response

{
"id": 1002,
"status": "Created"
}

## Error Codes

| Code | Description           |
| ---- | --------------------- |
| 200  | Success               |
| 400  | Bad Request           |
| 401  | Unauthorized          |
| 404  | Resource Not Found    |
| 500  | Internal Server Error |
