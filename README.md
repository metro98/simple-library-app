# Web-based Microservices Library Application

This is a microservices-based web application built with Flask, consisting of several independent services that communicate with each other using HTTP requests. The application demonstrates a simple book store with books and authors.

## Services

The application is composed of the following services:

1. **Book Service**: Handles book-related operations (get all books, get a specific book).
2. **Author Service**: Handles author-related operations (get all authors, get a specific author).
3. **API Gateway**: Acts as an entry point for clients and routes requests to the appropriate service.
4. **Web Frontend**: Serves the web application for users, interacting with the API Gateway to fetch and display data.

## Getting Started

### Prerequisites

- Docker
- Docker Compose (optional)

### Running the Application

1. Clone the repository:
2. Build the Docker images:
3. Start the containers:

This will start all the services as separate Docker containers and map the respective ports to the host machine.

4. Access the web application:

Once all the containers are running, you can access the web application by opening your web browser and navigating to `http://localhost:5003`.

### Service Discovery

This application uses a service registry (e.g., Consul or ZooKeeper) for service discovery, allowing the services to dynamically discover and communicate with each other without relying on hard-coded IP addresses or hostnames.

To set up the service registry, follow the instructions in the respective service registry documentation.

## Contributing

Contributions are welcome! If you find any issues or want to add new features, please open an issue or submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).