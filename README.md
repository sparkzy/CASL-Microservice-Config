# CASL-User-Config
Repository containing the cofniguration files for CASL microservices.

A microservice identifies which .yml file to use by checking the name of the .yml gfile.
Which ever .yml file matches the value in spring.application.name of the microservices own application.yml file will be used.

Ex:
the CASL-User-Service contains the following in it's aplication.yml:
spring:
  application:
    name: user-service
This will look at the "user-service.yml" file and use that as its configration file.
