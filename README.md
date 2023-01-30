# Architecture Design
Movie Service is a microservice based layered architectured RESTful Web Service. This service can be deployed independently on premise or any cloud platform.
Below are the different layers in this service:
##### API Layer
o	This is the top layer available for integration and interaction with front-end or end user to consume APIs
o	Request is validated at this layer. Spring Bean Validation take cares of all the validations at this layer. 

##### Service Layer
o	This layer sits in between API layer and Data access layer with some utility functionality
o	It is mainly responsible for interacting with Data Access Layer and transferring the recipes data as required by top and below layers
o	It's just another module added to decouple business logic of recipes data transfer and mapping from/to API layer

##### Data Access Layer
o	Responsible to provide Object Relationship Mapping (ORM) between higher level recipe Java objects and persistence layer tables
o	Springboot-starter-data-JPA module is used to implement mappings between objects and tables
o	This layer contains recipe entity classes and JPA repositories which implement lower level functionality of storing/retrieving recipes data
