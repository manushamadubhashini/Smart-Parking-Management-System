# Smart Parking Management System (SPMS)

A cloud-native, microservice-based platform for real-time parking space management and monitoring.

## Overview

The Smart Parking Management System addresses urban parking challenges by providing a scalable solution for:
- Real-time parking space availability tracking
- Dynamic space allocation and reservation
- Digital payment processing
- Vehicle entry/exit simulation
- Historical usage analytics

## Architecture

This system follows a microservices architecture built primarily with Spring Boot and Spring Cloud components:

### Core Infrastructure
- **Service Registry**: Eureka Server for service discovery
- **Configuration Server**: Spring Cloud Config for centralized configuration
- **API Gateway**: Spring Cloud Gateway as single entry point

### Business Services
- **Parking Space Service**: Manages parking spot availability and reservations
- **Vehicle Service**: Handles vehicle registration and tracking
- **User Service**: Manages user profiles and authentication
- **Payment Service**: Processes mock payments and generates receipts

## Technologies Used

- **Spring Boot** - Primary framework for microservices
- **Spring Cloud Eureka** - Service registry and discovery
- **Spring Cloud Config** - Configuration management
- **Spring Cloud Gateway** - API gateway
- **Spring Web** - RESTful API development
- **Postman** - API testing and validation

## Getting Started

### Prerequisites
- Java 11 or higher
- Maven 3.6+
- Git

### Running the Application

1. Clone the repository:
```bash
git clone git@github.com:manushamadubhashini/Smart-Parking-Management-System.git
cd smart-parking-management-system
```

2. Start services in the following order:
   - Eureka Server
   - Config Server
   - API Gateway
   - Business Services (Parking, Vehicle, User, Payment)

3. Access the Eureka Dashboard at `http://localhost:8761`

## API Testing

All APIs can be tested using the provided Postman collection. The system focuses exclusively on backend functionality without UI components.

## Key Features

- **Real-time Updates**: Dynamic parking space status updates
- **Scalable Architecture**: Microservices design for easy scaling
- **Digital Transactions**: Mock payment processing with receipt generation
- **Historical Tracking**: Usage logs and analytics
- **Multi-stakeholder Support**: Serves drivers, parking owners, and payment systems

## Business Objectives

- Enable real-time parking search and reservation
- Provide dynamic space management for parking owners
- Track usage analytics by city, zone, and owner
- Simulate vehicle entry/exit operations
- Handle secure payment processing
- Generate comprehensive historical logs
- Reduce traffic congestion and improve parking efficiency

## Resources

- [Postman Collections](https://github.com/manushamadubhashini/Smart-Parking-Management-System/blob/main/docs/postman%20(1).json)

- [Eureka Dashboard](https://github.com/manushamadubhashini/Smart-Parking-Management-System/blob/main/docs/screenShots/Screenshot%20(1115).png)

## Project Structure

```
smart-parking-management-system/
├── eureka-server/
├── config-server/
├── api-gateway/
├── parking-space-service/
├── vehicle-service/
├── user-service/
├── payment-service/
├── docs/
│   └── screenshots/
├── postman_collection.json
└── README.md
```

## Contributing

This project is part of a microservices architecture assignment focusing on smart city solutions and sustainable urban mobility.

## License

This project is developed for educational purposes as part of a microservices architecture implementation.
