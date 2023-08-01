# To-Do List API

This repository contains a simple Express.js application to manage a to-do list. The API provides endpoints for creating, retrieving, and updating to-do items. The data is stored in a local JSON file.

## Getting Started

### Prerequisites

- Node.js (v12.0.0 or higher)
- npm (v6.0.0 or higher)

### Installation

1. Clone the repository
2. Install dependencies
3.  Start the server

   The application should now be running at [http://localhost:3000](http://localhost:3000).

## API Endpoints

### GET `/`

Returns a welcome message.

### GET `/todos`

Fetches all to-do items. Optionally, use the `showPending` query parameter to filter incomplete to-dos:

- `/todos?showPending=1` will return only incomplete to-dos.

### PUT `/todos/:id/complete`

Marks a specific to-do item as complete.

### POST `/todos`

Creates a new to-do item. The request body must include a `name` field:

```json
{
 "name": "New To-Do Item"
}
