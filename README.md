## In Progress 
# Spring Boot with Filter
In this example, we're going to see how to write filter along with interceptor in Spring Boot REST API implementation.

You'll know:

1)How to configure Spring Data, JPA, Hibernate to work with Database<br>
2)How to define Data Models and Repository interfaces<br>
3)Way to create Spring Rest Controller to process HTTP requests<br>
4)Way to use Spring Data JPA to interact with H2 Database<br>
5)Way to use scheduler works

# Technical Details
In this project, we are going to use below set of versions for demonstrations.
```shell
Spring Boot - 3.3.4
Spring - 6.1.12
Lombok - 1.18.34
```
### Building

The example can be built with
```shell
mvn clean install
```

### Running the example in your local
```shell
mvn clean spring-boot:run
```
### Till this point, you won't find any difference as same data you inserted will be visible<br>
Now, lets insert the data into the Training Service. For this functionality demonstration, we have front end HTML page in place. Please verify the logs before invoking.

### Insert Data
http://localhost:8091/index.html

Please verify the logs after invoking.
Enter data and submit, verify logs.

### Retrieve all the inserted values
```shell
curl -X GET -H 'Content-Type: application/json' http://localhost:8091/training
```
### Retrieve Specific inserted values
```shell
curl -X GET -H 'Content-Type: application/json' http://localhost:8091/training/0
```
### Delete Specific inserted values
```shell
curl -X DELETE -H 'Content-Type: application/json' http://localhost:8080/training/0
```

