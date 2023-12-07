Microservices Architecture with Spring Cloud
Requirements:
Java 17
Docker
Steps to Run the Project Locally:
Clone the project:

bash
Copy code
git clone <project_repository_url>
Eureka Server:
Generate the Docker image for Eureka Server:

Navigate to the Eureka Server project:

bash
Copy code
cd "Architecture Micro Service avec Spring Cloud/Eureka server"
Package Eureka Server app into an executable JAR using Maven:

bash
Copy code
mvn package
Build a Docker image from the JAR file:

bash
Copy code
docker build -t eureka:0.1 .
Check Docker images:

bash
Copy code
docker images
API Gateway:
Generate the Docker image for the API Gateway:

Navigate to the Gateway project:

bash
Copy code
cd "Architecture Micro Service avec Spring Cloud/Gateway"
Package the Gateway app into an executable JAR using Maven:

bash
Copy code
mvn package
Build a Docker image from the JAR file:

bash
Copy code
docker build -t gateway:0.1 .
Check Docker images:

bash
Copy code
docker images