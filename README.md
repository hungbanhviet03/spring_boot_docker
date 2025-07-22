# Spring Boot Docker Sample

This is a sample Spring Boot application that can be built and run using Docker.

## Prerequisites

*   Java 17 or later
*   Maven
*   Docker

## Running the application with Maven

To run the application directly with Maven, use the following command:

```bash
./mvnw spring-boot:run
```

The application will be available at `http://localhost:8080`.

## Building and running with Docker

1.  **Build the application jar:**

    ```bash
    ./mvnw package
    ```

2.  **Build the Docker image:**

    ```bash
    docker build -t spring-boot-docker .
    ```

3.  **Run the Docker container:**

    ```bash
    docker run -p 8080:8080 spring-boot-docker
    ```

The application will be available at `http://localhost:8080`. 