# Decentralized Cluster-Based NoSQL Database

## Description

This project implements a distributed NoSQL database system built with Java, leveraging the power of Spring Boot, Maven, and Docker Compose. It offers efficient data management through:

- **JSON Data Representation:** Data is stored and manipulated using JSON, a widely adopted format for its flexibility and ease of use.
- **Data Partitioning:** Data is strategically distributed across nodes in the cluster for scalability and efficient access.
- **Load Balancing:** Nodes dynamically share the workload to ensure optimal performance under varying conditions.
- **Indexing:** Data is indexed to facilitate rapid retrieval and querying.
- **Optimistic Locking for Consensus:** This mechanism helps maintain data consistency across the decentralized cluster by preventing conflicting updates.
- **CRUD Operations via API:** The system provides a user-friendly API that enables basic data operations (Create, Read, Update, Delete) for interacting with the database.

## Microservices Architecture

The system adheres to a microservices architecture, promoting modularity and maintainability.

## Getting Started

### Prerequisites

- Java Development Kit (JDK) 17 or later ([Download JDK](https://www.oracle.com/java/technologies/downloads/))
- Maven ([Download Maven](https://archive.apache.org/dist/maven/maven-3/))
- Docker Desktop ([Install Docker Desktop](https://docs.docker.com/engine/install/))
- Docker Compose ([Install Docker Compose](https://docs.docker.com/compose/install/))

### Clone the Repository

- `git clone --recurse-submodules -j8 https://github.com/Jafar-ibrahim/Decentralized-Cluster-Based-NoSQL-DB-System`
- `cd Decentralized-Cluster-Based-NoSQL-DB-System`

### Build the Project

mvn clean install


### Run the Database Cluster

1. Open a terminal window within the project directory.
2. Run `docker-compose up -d` to start the cluster in detached mode. This will build and launch the necessary Docker containers for each service.

### Access the API

-Once the cluster is running, you can interact with the database through the provided API using tools like Postman or curl. 
-Database Nodes URL : http://host.docker.internal:900[2-5]
-Task Assignment App (Demo App) URL : http://host.docker.internal:9090/task-app/api/auth/login

## Developing and Contributing

If you're interested in contributing to this project, feel free to fork the repository on GitHub and create pull requests with your enhancements or bug fixes.

## Disclaimer

This project is provided as-is for educational and demonstration purposes. While it showcases core concepts of a decentralized NoSQL database, it might require further development for production-grade implementation. Consider incorporating additional features like security best practices, comprehensive testing suites, and monitoring/logging mechanisms for a more robust solution.
