# MongoDB API Connection Guide

This document provides all the necessary details to connect to and interact with the MongoDB Management API.

## Base Information

- **Base URL**: `https://apis.inventechsolution.com`
- **Documentation**: `https://apis.inventechsolution.com/docs` (Requires Admin Password)

## Authentication

The API uses a two-tier authentication system:

### 1. Global API Key (Required for all `/api` requests)
All API requests (except health checks) require an API key passed in the headers.
- **Header Name**: `X-API-Key`
- **API Token**: `c452e7766b1237e1dafdb23a4f3b149898f0daf279f67f5ec0f9b7880a0a62bd`

### 2. Database Authentication (Required for most operations)
Operations on specific databases, collections, or documents require database-level credentials. These are the credentials created when the database was initialized (or the admin root credentials).
- **Header Name**: `x-db-username`
- **Header Name**: `x-db-password`

---

## API Endpoints

### 1. Database Operations

| Method | Endpoint | Auth Level | Description |
| :--- | :--- | :--- | :--- |
| `GET` | `/api/databases` | API Key | List all databases on the server |
| `GET` | `/api/databases/:dbName` | API Key | Get detailed stats and collection list for a database |

---

### 2. Collection Operations

> **Note**: All collection operations require **API Key** AND **Database Auth** headers.

| Method | Endpoint | Description |
| :--- | :--- | :--- |
| `GET` | `/api/collections/:dbName` | List all collections in a specific database |
| `GET` | `/api/collections/:dbName/:collectionName` | Get collection stats and index details |
| `POST` | `/api/collections/:dbName/:collectionName` | Create a new collection |
| `DELETE` | `/api/collections/:dbName/:collectionName` | Drop a collection |

---

### 3. Document Operations (CRUD)

> **Note**: All document operations require **API Key** AND **Database Auth** headers.

| Method | Endpoint | Description |
| :--- | :--- | :--- |
| `GET` | `/api/documents/:dbName/:collectionName` | Get documents with pagination/filtering |
| `GET` | `/api/documents/:dbName/:collectionName/:id` | Get a specific document by its `_id` |
| `POST` | `/api/documents/:dbName/:collectionName` | Create a single new document |
| `POST` | `/api/documents/:dbName/:collectionName/bulk` | Insert multiple documents at once |
| `PUT` | `/api/documents/:dbName/:collectionName/:id` | Replace a document entirely |
| `PATCH` | `/api/documents/:dbName/:collectionName/:id` | Update specific fields in a document |
| `DELETE` | `/api/documents/:dbName/:collectionName/:id` | Delete a specific document |
| `DELETE` | `/api/documents/:dbName/:collectionName` | Delete multiple documents matching a filter |

#### Query Parameters for `GET /api/documents`
- `page`: Page number (default: 1)
- `limit`: Documents per page (default: 100, max: 1000)
- `sortBy`: Field to sort by (default: `_id`)
- `sortOrder`: `asc` or `desc`
- `filter`: URL-encoded JSON string (e.g., `?filter={"status":"active"}`)
- `fields`: Comma-separated list of fields to return

---

## Health & System

| Method | Endpoint | Description |
| :--- | :--- | :--- |
| `GET` | `/health` | Check service status (Public) |
| `GET` | `/` | API version and overview (Public) |
