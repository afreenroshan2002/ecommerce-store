# E-commerce Application

[![Build Status](https://travis-ci.com/prasadus92/registration-service.svg?branch=master)](https://travis-ci.com/prasadus92/ecommerce-store) [![codecov](https://codecov.io/gh/patrykkrawczyk/TDDAndDesignPatternsExample/branch/master/graph/badge.svg)](https://codecov.io/gh/prasadus92/ecommerce-store) [![Maintainability](https://api.codeclimate.com/v1/badges/9ef32de1cfdbcc97b1f0/maintainability)](https://codeclimate.com/github/prasadus92/ecommerce-store/maintainability)

## Problem Statement

Create a tiny REST/JSON web service in Java using Spring Boot (RestController) with an API that
supports basic Products' CRUD:

- Create a new Product

- Get a list of all Products

- Update a Product

The API should also support:

- Placing an Order

- Retrieving all orders within a given time period

A product should have a name and some representation of its price.

Each order should be recorded and have a list of products. It should also have the buyer’s e-mail, and the
time the order was placed. The total value of the order should always be calculated, based on the prices
of the products in it.

It should be possible to change the product’s price, but this shouldn’t affect the total value of orders which
have already been placed.

### Requirements

- Implement your solution according to the above specification.

- Provide unit tests.

- Document your REST-API.

- Provide a storage solution for persisting the web service’s state.


## Solution Overview

### Tools Used

- Java 11

- Spring Boot v2.2.4.RELEASE

- Maven

- Travis (CI)

## Clone the Repository
Navigate to the directory where you want to clone the project and run:
```bash
git clone git@github.com:afreenroshan2002/ecommerce-store.git
cd ecommerce-store
```
## Building the Application

As the project uses Maven as the build system, just run the below command in the project directory -

```bash
mvn clean install
```

The name of the generated JAR is `ecommerce-store-application.jar`.


### Running Tests

Run the below command -

```bash
mvn clean test
```

## Running the Application

### Using Maven

You could use Maven to run the Spring Boot application; here is the command to use -

```bash
mvn spring-boot:run
```

### Using the generated artifact

Once you build the Application, the artifacts will be generated and copied to `target` directory. Hence, using the JAR, we could start the Application this way -

```bash
java -jar ecommerce-store-application.jar
```


## Accessing the API Documentation

Swagger is included in the project. Hence, the API documentation is available at http://localhost:8080/swagger-ui.html. 

