## Spring Boot  Persistence
#### Franciso Javier Rojas Muñoz

---

### H2

Configure pom.xml
```
    <dependency>
        <groupId>org.springframework.boot</groupId>
        <artifactId>spring-boot-starter-web</artifactId>
    </dependency>

    <dependency>
        <groupId>org.springframework.boot</groupId>
        <artifactId>spring-boot-starter-data-jpa</artifactId>
    </dependency>

    <dependency>
        <groupId>com.h2database</groupId>
        <artifactId>h2</artifactId>
        <scope>runtime</scope>
    </dependency>
```
Configure application properties:
```
    spring.datasource.url=jdbc:h2:mem:testdb
    spring.jpa.defer-datasource-initialization=true
    spring.h2.console.enabled=true
    spring.datasource.driverClassName=org.h2.Driver
    spring.datasource.username=sa
    spring.datasource.password=
    spring.jpa.database-platform=org.hibernate.dialect.H2Dialect
```
Configure the entity
![](.README_images/c0288ad7.png)

and run it
![](.README_images/ebde5c3e.png)
