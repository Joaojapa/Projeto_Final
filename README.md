# Express API for Book Management

This project is a RESTful API built with Express.js to manage a collection of books. It implements CRUD operations and includes JWT authentication for secure access.

## Features

- **CRUD Operations**: Create, Read, Update, and Delete books.
- **JWT Authentication**: Secure routes with JSON Web Tokens.
- **Error Handling**: Centralized error handling middleware.
- **Environment Configuration**: Use of `.env` for sensitive information.

## Project Structure

```
express-api
├── src
│   ├── app.js                # Initializes the Express application
│   ├── server.js             # Starts the server
│   ├── controllers           # Contains controller logic for handling requests
│   │   └── bookController.js
│   ├── routes                # Defines API routes
│   │   ├── bookRoutes.js
│   │   └── authRoutes.js
│   ├── middleware            # Middleware functions for authentication and error handling
│   │   ├── authMiddleware.js
│   │   └── errorHandler.js
│   ├── models                # Database models
│   │   └── bookModel.js
│   ├── config                # Configuration files
│   │   └── database.js
│   └── utils                 # Utility functions
│       └── jwt.js
├── .env                      # Environment variables
├── .gitignore                # Files to ignore in Git
├── package.json              # Project metadata and dependencies
└── README.md                 # Project documentation

## Funcionalidades
- CRUD de Produtos
- Autenticação JWT
- Validações de entrada
- Testes unitários e de integração
- Documentação com Swagger

## Tecnologias
- Node.js
- Express
- MongoDB (driver nativo)
- JWT
- Jest + Supertest

## Como rodar

```bash
git clone <repo>
cd product-manager-api
npm install
cp .env.example .env
npm run dev
```

## Installation

1. Clone the repository:
   ```
   git clone <repository-url>
   cd express-api
   ```

2. Install dependencies:
   ```
   npm install
   ```

3. Create a `.env` file in the root directory and add your environment variables:
   ```
   DATABASE_URL=<your_database_url>
   JWT_SECRET=<your_jwt_secret>
   ```

4. Start the server:
   ```
   npm start
   ```

## API Endpoints

### Books

- **GET /api/books**: Retrieve all books
- **GET /api/books/:id**: Retrieve a book by ID
- **POST /api/books**: Create a new book
- **PUT /api/books/:id**: Update a book by ID
- **DELETE /api/books/:id**: Delete a book by ID

### Authentication

- **POST /api/auth/register**: Register a new user
- **POST /api/auth/login**: Log in a user and receive a JWT

## License

This project is licensed under the MIT License.