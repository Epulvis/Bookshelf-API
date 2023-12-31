**Description:**
This JavaScript code defines a simple CRUD (Create, Read, Update, Delete) API for managing a collection of books using the Hapi.js framework. The API exposes endpoints for adding, retrieving, updating, and deleting books. It utilizes the `@hapi/hapi` library for creating an HTTP server and the `nanoid` library for generating unique identifiers.

**Endpoints:**
1. **POST:**
   - Adds a new book to the collection.
   - Validates incoming data and responds with success or failure messages.

2. **GET:**
   - Retrieves a list of books based on optional query parameters (name, reading, finished).
   - Filters books based on the query parameters and responds with a formatted list of books.
   - Retrieves a specific book by its unique identifier (bookId).
   - Responds with the details of the requested book or a failure message if the book is not found.

4. **PUT:**
   - Updates the details of a specific book identified by its unique identifier (bookId).
   - Validates incoming data, checks for the existence of the book, and responds with success or failure messages.

5. **DELETE:**
   - Deletes a specific book from the collection based on its unique identifier (bookId).
   - Responds with success or failure messages based on the outcome of the deletion.

**Data Structure:**
- Books are represented as objects with properties like `id`, `name`, `year`, `author`, `summary`, `publisher`, `pageCount`, `readPage`, `reading`, `finished`, `insertedAt`, and `updatedAt`.
- The collection of books is stored in memory as an array named `books`.

**Usage:**
- The server is configured to run on port 9000 and the localhost.
- The server logs its status message upon successful startup.

**Error Handling:**
- The code includes basic error handling for invalid requests or unhandled rejections.

This code provides a foundation for building a book management API with basic validation and error handling.

---
