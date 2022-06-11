# springboot-mongodb
#### A basic Spring Boot REST application that uses mongodb

### Configuring mongodb with spring boot
#### Dependency
```
<dependency>
    <groupId>org.springframework.boot</groupId>
	<artifactId>spring-boot-starter-data-mongodb</artifactId>
</dependency>
```
#### application.properties
Before this step you need to setup and create cluster in Mongodb Atlas. Find reference at the nd of the page.
```
mongodb.database=employee
mongodb.connection.string=mongodb+srv://user:Password@scluster.promp8q.mongodb.net/?retryWrites=true&w=majority
```
#### Add Mongo Client configuration using the above properties

### Model for Mongodb
Has @Document("name") instead of Entity/Table like in JPA. Document Name is the name of the table created in database.

#### References
- [Getting Started with Mongodb Atlas](https://www.mongodb.com/docs/atlas/getting-started/)
- [https://medium.com/bb-tutorials-and-thoughts/how-to-build-rest-api-with-spring-boot-and-mongodb-d8ebc658ffe3](https://medium.com/bb-tutorials-and-thoughts/how-to-build-rest-api-with-spring-boot-and-mongodb-d8ebc658ffe3)