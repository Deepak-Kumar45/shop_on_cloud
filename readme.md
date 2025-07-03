# SmartSync Microservices Architecture

This is a full-stack microservices-based backend for SmartSync — a contact management application.

## Services:
- `auth-service`: Authentication & JWT
- `contact-service`: Manages contacts
- `notification-service`: Email/SMS
- `api-gateway`: Routes & filters
- `service-discovery`: Eureka registry
- `config-service`: Centralized configs

## How to Run

1. Start Eureka server: `cd service-discovery && mvn spring-boot:run`
2. Start Config server: `cd config-service && mvn spring-boot:run`
3. Start other services one by one.
4. Optionally: use `docker-compose up` to run everything (if Dockerized).
