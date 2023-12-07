# Architecture_Microservices_SpringCloud

# Requirement :
Java 17 + docker 
# Follow this steps to run the project lcoally
1)  open your terminal and clone this project
2)  generate the docker image for eureka server 
    - go inside the eureka server project 
    >cd "Architecture Micro Service avec Spring Cloud/"Eureka server""
    - package eureka server app into an executable jar using your editor or by typing :
    >mvn package 

    ![img_2.png](img_2.png)

    - build a docker image from this jar file by typing:
    > docker build -t eureka:0.1 .
    - check your docker images by typing in your cmd:
    > docker images 
    
    ![img.png](img.png)
    + know we have a docker image for our  eureka server  application
    
3)   generate the docker image for the API GATEWAY 
     - go inside the Gateway project
    ![img_1.png](img_1.png)
     - package gateway  app into an executable jar using your editor or by typing :
     > mvn package
     - build a docker image from this jar file by typing:
     > docker build -t gateway:0.1
     - check your docker images by typing in your cmd:
     > docker images
     + know we have a docker image for our  API GATEWAY  application
4) generate the docker image for the service client 
    - go inside the ServiceClient Folder and package the app into an executable jar using your editor or by typing :
    > mvn package
    - build a docker image from this jar file by typing:
     > docker build -t clients:0.1
    - check your docker images by typing in your cmd:
     > docker images
   + know we have a docker image for our  service client  application
5) generate the docker image for the service voiture:
    - go inside the voiture Folder and package the app into an executable jar using your editor or by typing :
   > mvn package
    - build a docker image from this jar file by typing:
   > docker build -t voitures:0.1
    - check your docker images by typing in your cmd:
   > docker images
    + know we have a docker image for our  service voiture  application
    
    