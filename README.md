<div align="center">
  <h1>🌐 Bitlord's Computer Parts - Eureka Service Registry</h1>
  <p>The centralized service discovery and registration server for the microservices cluster.</p>
</div>

## 📖 Overview
The **Eureka Server** is the heart of the microservices topology. Rather than hardcoding IP addresses and ports, all services (API Gateway, Auth, Order, Inventory, Notification) register themselves with Eureka upon startup. This allows for dynamic scaling, load balancing, and resilient service-to-service communication.

[⬅️ Back to Main Repository](https://github.com/yourusername/bitlord-computer-parts)

## 🛠️ Tech Stack
- **Language**: Java 17
- **Framework**: Spring Boot 3.2
- **Service Discovery**: Spring Cloud Netflix Eureka Server

## 🎛️ Dashboard
Eureka provides a web-based UI to monitor the health and status of all registered microservice instances.
- **URL**: `http://localhost:8761/`

## 🚀 How to Run Locally

### Prerequisites
- JDK 17
- Maven

### Steps
1. Navigate to the `eureka-server` directory.
2. Build the project:
   ```bash
   mvn clean install -DskipTests
   ```
3. Run the application:
   ```bash
   mvn spring-boot:run
   ```
4. The Eureka dashboard will be available on port `8761`. **This must be the first service started in the infrastructure.**
