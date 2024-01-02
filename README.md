# Simple Book Inventory Management API

This is a simple RESTful API for managing a book inventory. It allows you to perform basic CRUD operations (Create, Read, Update, Delete) on a collection of books.

## Getting Started

To run the application, follow these steps:

1. Clone the repository:

   ```bash
   git clone https://github.com/sinouw/golang-rest-books
   cd golang-rest-books

   ```  

2. Install the required dependencies:

   ```bash
   go get -u github.com/gin-gonic/gin
   ```
   
3. Run the application:

   ```bash
   go run main.go
   ```

# API Endpoints

## Get All Books
- **Method:** GET
- **Endpoint:** `/books`
- **Description:** Get a list of all books.
- **cURL Request:**
  ```bash
  curl -X GET http://localhost:3000/books
  ```

## Get Specific Book
- **Method:** GET
- **Endpoint:** `/books/:id`
- **Description:** Get details of a specific book by ID.
- **cURL Request:**
  ```bash
  curl -X GET http://localhost:3000/books/1

  ```

## Create New Book
- **Method:** POST
- **Endpoint:** `/books`
- **Description:** Create a new book.
- **cURL Request:**
  ```bash
  curl -X POST http://localhost:3000/books -H "Content-Type: application/json" -d '{"title": "The Great Gatsby", "author": "F. Scott Fitzgerald", "Quantity": 10}'
  ```

## Update Book Details
- **Method:** PUT
- **Endpoint:** `/books/:id`
- **Description:** Update details of a specific book by ID.
- **cURL Request:**
  ```bash
  curl -X PUT http://localhost:3000/books/1 -H "Content-Type: application/json" -d '{"title": "The Great Gatsby", "author": "F. Scott Fitzgerald", "Quantity": 10}'
  ```

## Delete Book
- **Method:** DELETE
- **Endpoint:** `/books/:id`
- **Description:** Delete a book by ID.
- **cURL Request:**
  ```bash
  curl -X DELETE http://localhost:3000/books/1
  ```

# Contributing

Feel free to contribute to this project! Your feedback and contributions are welcome.

## How to Contribute

If you would like to contribute to the project, consider the following steps:

1. **Opening Issues:**
   - If you find a bug or have a feature request, please open an issue to discuss it.
   - Provide clear and detailed information, including steps to reproduce any bugs.

2. **Pull Requests:**
   - Feel free to submit pull requests for bug fixes or new features.
   - Fork the repository, create a branch, make your changes, and submit a pull request.
   - Ensure your code follows the project's coding standards.

3. **Feature Requests:**
   - If you have ideas for new features, open an issue to discuss them.
   - Provide context and rationale for the proposed feature.

4. **Code Reviews:**
   - Participate in code reviews to help improve the overall quality of the project.

## Contributors

A big thank you to all the contributors who have helped improve this project!

Happy contributing!