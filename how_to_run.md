# Setup guide
----
##### Minimum Requirements
-  Java 11
-  Maven 3.x
##### Install the application
1. Make sure you have Java and Maven installed
2. Open the command line in the source code folder
3. Build project
   `$ mvn package`
 4. Run the test cases
    `$ mvn test`
5.  Go inside target folder
    `$ cd target`
5. Run the project
   `$ java -jar movie-service-0.0.1-SNAPSHOT.jar`
6. Open the swagger-ui with the link below
`http://localhost:9080/movie-service/swagger-ui.html#/`
7. Actuator end point
`http://localhost:9090/movie-service/management`
