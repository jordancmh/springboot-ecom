# Springboot-Ecom

This is an oversimplified backend ecommerce project using Spring Boot & H2 in-memory database. This project's primary
purpose is to serve as a learning experience for Spring Boot, separation of concerns with the
Controler-Service-Repository pattern, API design, Image file uploading/downloading, and JPA integration.

## Features

- Creates a database in H2 with a single entity named Product.
- CRUD operations facilitated by API endpoints, managed by a single controller class.
- A search feature that looks for an occurence of a keyword in the name, brand, category and description columns within
  the Product table.

## Dependencies

- Java 21
- Spring Boot 3.4.4
- Spring Data JPA
- Spring Boot DevTools
- H2 database
- Lombok

## API Reference

#### Product Controller (`/api`)

| Method | URL                          | Description                                        |
|:-------|:-----------------------------|:---------------------------------------------------|
| GET    | `/products`                  | Retrieve a list of all products                    |
| GET    | `/product/{id}`              | Retrieve a product by ID                           |
| POST   | `/product`                   | Add a product and its image                        |
| GET    | `/product/{productId}/image` | Retrieve a product's image using its ID            |
| PUT    | `/product/{productId}`       | Update a product and its image                     |
| DELETE | `/product/{productId}`       | Delete a product by ID                             |
| GET    | `/products/search`           | Search for a product via `keyword` input parameter |

## License

[MIT](https://choosealicense.com/licenses/mit/)
