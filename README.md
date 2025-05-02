
# Springboot-Ecom

This is an oversimplified backend ecommerce project using Spring Boot & H2 in-memory database. This project's primary purpose is to serve as a learning experience for Spring Boot, separation of concerns with the Controler-Service-Repository pattern, API design, Image file uploading/downloading, and JPA integration.

## Features
- Creates a database in H2 with a single entity named Product.
- CRUD endpoints which are managed by a single controller class.
- A search feature that looks for an occurence of a keyword in the name, brand, category and description columns from the Product table.

## Dependencies

- Java 21
- Spring Boot 3.4.4
- Spring Data JPA
- Spring Boot DevTools
- H2 database
- Lombok

## License

[MIT](https://choosealicense.com/licenses/mit/)
