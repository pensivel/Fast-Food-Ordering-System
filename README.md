# Fast Food – Online Food Ordering System

An online food ordering platform developed using a Microservices architecture. The system allows customers to browse restaurants, order food, make online payments and track deliveries, while administrators manage restaurants, orders, customers and transactions.

## Project Overview

This project was developed as part of the Service-Oriented Software Development coursework at Hanoi University of Industry.

The system is designed around independent backend services that communicate through RESTful APIs, with centralized API routing and service discovery.

## Technology Stack

**Backend**
- Java
- Spring Boot
- Spring Cloud Gateway
- Netflix Eureka
- Maven

**Frontend**
- HTML5
- CSS3
- JavaScript

**Database**
- MySQL

**Tools**
- IntelliJ IDEA
- Visual Studio Code
- Postman
- Apache JMeter
- Git and GitHub
- Docker (service configuration)

## System Architecture

The backend contains the following services:

| Service | Responsibility |
|---|---|
| Auth Service | User authentication and registration |
| Customer Service | Customer information management |
| Restaurant Service | Restaurant and food management |
| Order Service | Order creation and management |
| Payment Service | Payment processing and VNPay integration |
| Delivery Service | Delivery and shipment tracking |
| Eureka Server | Service registration and discovery |
| API Gateway | Centralized API routing |

## Main Features

### Customer Features
- User registration and login
- Browse restaurants and food menus
- Search for restaurants and dishes
- Add, update and remove cart items
- Place food orders
- Online payment integration with VNPay
- Track order and delivery status
- Submit food and restaurant reviews

### Administrator Features
- Dashboard and revenue statistics
- Restaurant management
- Food and menu management
- Customer management
- Order management
- Payment transaction management
- Delivery management

## Database Design

The system follows the Database-per-Service approach described in the project design, where services manage their own business data.

The main business entities include:
- Users
- Restaurants
- Dishes
- Orders
- Payments
- Deliveries

## Testing

The project report describes API and performance testing scenarios using:
- Postman
- Apache JMeter

Testing scenarios cover payment creation, VNPay IPN callbacks, order processing, restaurant management and delivery operations.

## Project Structure

```text
Fast-Food-Ordering-System/
│
├── Backend/
│   ├── auth_service/
│   ├── customer_service/
│   ├── restaurant_service/
│   ├── order_service/
│   ├── payment_service/
│   ├── delivery_service/
│   ├── eureka_server/
│   └── gateway/
│
├── Frontend/
│   ├── admin/
│   ├── auth/
│   ├── customer/
│   ├── delivery/
│   ├── order/
│   ├── payment/
│   ├── restaurant/
│   ├── css/
│   └── js/
│
├── index.html
└── README.md
```

## Running the Project

The backend services are managed independently using Maven.

General setup requirements:
1. Install a compatible JDK and Maven.
2. Install and configure MySQL.
3. Configure database connections for each service.
4. Start Eureka Server.
5. Start the API Gateway.
6. Start the business services.
7. Open the frontend in a web browser.

Detailed configuration and startup instructions should be completed after verifying the service configurations.

## Project Background and Maintainer

This repository is an authorized portfolio copy of an existing university group project.

**Current Repository Maintainer:** Khanh Nguyen

The original project was developed as a group coursework project. This repository is maintained separately for learning, further development and portfolio purposes.

## License

Usage and distribution are subject to the permission and transfer terms provided by the original project owner.