# Projects
- [Epaper Service](https://github.com/manish24-tech/spring-boot-with-docker/tree/main/EpaperService) - manage news papers details.

## Prerequisites
- Java 17
- Maven 3.8.6
- Docker 20.10.22

## Technologies

- Java
- Spring Boot
- Docker

## Setup

1. Clone the repository and navigate to root directory

# Running the Application Manually

2. Install dependencies: `mvn clean install`

3. start the application: `java -jar target/<jar-name>.jar`

# Running the Application with Docker

4. Build the Docker image: `docker build -t epaper-service:1.0 .`
5. Start the Docker container: `docker run --name spring-boot-container -p 8080:8080 -t epaper-service:1.0`
6. Access the application at `http://localhost:8080`
7. Start the Docker in case it stoped: `docker start epaper-service:1.0`
8. Stop the Docker in case it running: `docker stop epaper-service:1.0`
9. Access the API docunmentation UI at `http://localhost:8080/swagger-ui/index.html#` 

## Configuration
- `application.properties`: update database properties with MySQL. currently it's configured with H2 databse.

## Troubleshooting
- If the application fails to start, make sure that the correct version of Java is installed and that the `JAVA_HOME` environment variable is set.
- If the Docker container fails to start, check the Docker logs for error messages and make sure that the container has access to the required ports and resources.

## License
This project is licensed under the [MIT License](https://opensource.org/licenses/MIT) - see the LICENSE file for details.
