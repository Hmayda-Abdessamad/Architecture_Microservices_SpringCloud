# Architecture_Microservices_SpringCloud

# Requirement :
Java 17 + docker

# Project Overview:

This Spring Boot-based microservices project comprises two microservices, namely clients and voitures. The voitures service can communicate with the clients service using the Feign client. Additionally, there's an Eureka server and a gateway (Eureka Gateway) that manage service registration and API routing, respectively. All components of this project are containerized using Docker.

# Key Components:

1) Microservices:

- Clients Service: A microservice handling client-related functionalities.
- Voitures Service: A microservice capable of communicating with the Clients service via the Feign client.

2) Eureka Server and Gateway:

 - Eureka Server:Responsible for service registration and discovery.
 - Gateway (Eureka Gateway):Manages API routing and acts as a gateway to the microservices.
3) Databases:Each microservice (clients and voitures) utilizes its own PostgreSQL database instance.

# Global Architecture :
![Architecture Microservices.png](..%2F..%2FArchitecture%20Microservices.png)

# Run the project :
1) go to the root folder of the project "Architecture Micro Service avec Spring Cloud" where the docker-compose.yaml file is located 
2) type :
  > docker compose up

- this will take time 

3) you will find 6 docker container running like this image from docker desktop shows: 
![img_7.png](img_7.png)
4) go to the ui of eureka server , you will find 3 instances :
![img_8.png](img_8.png)
5) so all is good know  we have to test our two services by going to :
- ![img_9.png](img_9.png)
- ![img_10.png](img_10.png)