# BiblioNovaa

BiblioNovaa is a comprehensive web application designed for efficient library management, featuring seamless synchronization between MongoDB and Neo4j databases. This application allows for the streamlined management of books, members, loans, and returns.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)


## Features

- **Book Management**: Add, list, modify, and delete books.
- **Member Management**: Add, list, modify, and delete members.
- **Loan Management**: Record and track book loans.
- **Database Synchronization**: Ensure data consistency between MongoDB and Neo4j.
- **User Authentication**: Secure login system for library staff.

## Installation

### Prerequisites

- Python 3.7+
- Flask
- MongoDB
- Neo4j
- Git

### Steps

1. Clone the repository:
    ```bash
    git clone https://github.com/MehdiBoukhobza/BiblioNovaa.git
    cd BiblioNovaa
    ```

2. Create a virtual environment and activate it or add one automatically using PyCharm:
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. Install the required packages:

4. Set up MongoDB and Neo4j:
    - Ensure MongoDB is running on your machine or server.
    - Ensure Neo4j is running and accessible.
    
    For MongoDB:
    ```bash
    docker pull mongodb/mongodb-community-server:latest
    docker run --name mongodb -p 27017:27017 -d mongodb/mongodb-community-server:latest
    ```
    
    For Neo4j:
    ```bash
    docker pull neo4j
    docker run --name myneo4j -p 7687:7687 -p 7474:7474 -d -e NEO4J_AUTH=neo4j/password neo4j:latest
    ```

5. Run the application:
    ```bash
    flask run
    ```

## Usage

- Access the application at `http://127.0.0.1:5000`.
- Use the navbar to navigate through different sections of the application.
- Manage books, members, and loans using the provided interfaces.
- Use the login page to access admin functionalities.
- To add an admin, you need to change the role from the MongoDB database.

## Contributing

We welcome contributions! Please follow these steps to contribute:

1. Fork the repository.
2. Create a new branch:
    ```bash
    git checkout -b feature/your-feature-name
    ```
3. Make your changes.
4. Commit your changes:
    ```bash
    git commit -m 'Add some feature'
    ```
5. Push to the branch:
    ```bash
    git push origin feature/your-feature-name
    ```
6. Open a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
