# API Gateway Service

## Description
This service acts as the entry point for the microservices architecture. It handles routing requests to the appropriate backend services using Spring Cloud Gateway.

## Features
- Request Routing
- Load Balancing (via Eureka)
- Centralized access to Products, Orders, and Payments.

## Port
- Default: `8080`

## Endpoints
- `/productos/**`: Proxies to Product Service
- `/ordenes/**`: Proxies to Order Service
- `/pagos/**`: Proxies to Payment Service

## Infrastructure Repo
- [Main Infrastructure & Orchestration](https://github.com/UniModelo-Projects/Vacaciones_Microservices_Infrastructure)
