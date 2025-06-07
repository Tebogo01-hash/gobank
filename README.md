# GoBank: A Simple Banking Backend Project 🚀

![GoBank](https://img.shields.io/badge/GoBank-Backend%20Development-blue)

Welcome to the GoBank repository! This project serves as a practical introduction to backend development using Go. Here, you will find a simple banking application that helps you get hands-on experience with Go and its ecosystem. 

## Table of Contents

- [Project Overview](#project-overview)
- [Technologies Used](#technologies-used)
- [Features](#features)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)
- [Releases](#releases)

## Project Overview

GoBank is a straightforward project aimed at helping developers familiarize themselves with backend development in Go. It covers essential concepts and best practices, providing a solid foundation for further exploration in Go's ecosystem. Whether you are new to Go or looking to sharpen your skills, this project is for you.

## Technologies Used

- **Go**: The programming language for building the backend.
- **PostgreSQL**: The database used for storing user and transaction data.
- **Redis**: A caching layer to improve performance.
- **Fiber**: A web framework for building the API.
- **GraphQL**: For flexible data querying.
- **Migration Tools**: For managing database changes.

## Features

- User registration and authentication
- Account management
- Transaction history
- Caching with Redis
- GraphQL API for data queries
- PostgreSQL database for persistent storage
- Migration scripts for database management

## Getting Started

To get started with GoBank, follow these steps:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/Tebogo01-hash/gobank.git
   cd gobank
   ```

2. **Install dependencies**:
   Ensure you have Go installed. You can use the following command to install the required packages:
   ```bash
   go mod tidy
   ```

3. **Set up the database**:
   Make sure you have PostgreSQL installed. Create a database for GoBank and update the connection string in the `.env` file.

4. **Run migrations**:
   Use the migration tool to set up the database schema:
   ```bash
   go run migrations/migrate.go
   ```

5. **Start the server**:
   Launch the application with:
   ```bash
   go run main.go
   ```

## Usage

Once the server is running, you can interact with the API using tools like Postman or curl. Here are some example requests:

- **Register a new user**:
  ```http
  POST /api/register
  Content-Type: application/json

  {
      "username": "exampleUser",
      "password": "examplePassword"
  }
  ```

- **Get transaction history**:
  ```http
  GET /api/transactions
  Authorization: Bearer <token>
  ```

For a complete list of API endpoints, refer to the documentation within the codebase.

## Contributing

Contributions are welcome! If you want to help improve GoBank, feel free to fork the repository and submit a pull request. Here are some ways you can contribute:

- Report bugs
- Suggest features
- Improve documentation
- Write tests

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Contact

For any questions or suggestions, feel free to reach out:

- **GitHub**: [Tebogo01-hash](https://github.com/Tebogo01-hash)

## Releases

To download the latest version of GoBank, visit the [Releases](https://github.com/Tebogo01-hash/gobank/releases) section. Here, you can find compiled binaries and other resources.

## Conclusion

Thank you for checking out GoBank! This project is an excellent way to get familiar with Go and backend development practices. Feel free to explore, learn, and contribute. Happy coding!