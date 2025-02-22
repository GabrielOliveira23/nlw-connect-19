# Event Subscriber Tracker 🚀

A server built with Node.js and TypeScript to manage **subscribers** for events. Each subscriber is assigned a unique link that tracks and ranks the number of accesses generated by them.

## ✨ Features

- Register subscribers for events.
- Automatically generate unique links for each subscriber.
- Track link access counts.
- Rank subscribers based on the accesses they generate.
- Well-structured and typed APIs using TypeScript.
- Interactive API documentation with Swagger.
- Efficient data management using PostgreSQL and Redis.

## 🛠️ Technologies Used

- **Node.js**: JavaScript runtime environment on the server.
- **TypeScript**: A superset of JavaScript for enhanced safety and scalability.
- **PostgreSQL**: Relational database for persistent data storage.
- **Redis**: In-memory cache for tracking accesses and optimized performance.
- **Drizzle ORM**: Simplified and efficient database management.
- **Drizzle Kit**: CLI tool for database migrations.
- **Docker**: Containerization to standardize development and production environments.
- **Swagger**: Tool for interactive API documentation.

## 📦 Installation and Setup

### Prerequisites

Make sure you have the following tools installed:

- [Node.js](https://nodejs.org/)
- [Docker](https://www.docker.com/)
- [Docker Compose](https://docs.docker.com/compose/)

### Steps

1. Clone the repository:

    ```bash
      git clone https://github.com/GabrielOliveira23/event-subscriber-ranker.git
      cd event-subscriber-ranker
    ```

2. Copy the .env.example file to .env and configure the environment variables:

    ```bash
      cp .env.example .env
    ```

3. Start the services with Docker Compose:

    ```bash
      docker-compose up -d
    ```

4. Install the project dependencies:

    ```bash
      npm install
    ```

5. Run the database migrations:

    ```bash
      npx drizzle-kit generate
      npx drizzle-kit migrate
    ```

6. Start the development server:

    ```bash
      npm run dev
    ```

The server will be available at <http://localhost:4000>.

## 📚 API Documentation

The interactive API documentation is available through Swagger after starting the server. Access it at: <http://localhost:4000/docs>
