# Credit Score Analysis Tool

### Overview
This prototype project demonstrates a microservice architecture with three microservices: 
1. **CreditScoringService** - Manages credit score calculation and caching.
2. **UserManagement** - Handles user registration and login with OAuth2.
3. **SpringCloudGateway** - Routes requests between the frontend and microservices.

> **Note**: This is a simplified prototype to explain the integration of various tools and concepts like Redis, Kafka, Log4j2, Splunk, and OAuth2. It may not fully function as an enterprise-ready application.

---

### Project Structure
- **`src/main/java`**: Main code of the application.
- **`src/main/resources`**: Configuration files (e.g., `application.properties`).
- **`src/test/java`**: Test cases for validation.
- **`pom.xml`**: Dependency configuration.

---

### Key Features
#### 1. **Redis Integration**
- Caching with Redis in `CreditScoringService`.
- Configuration: `application.properties` and a dedicated config class.
- Usage: `RedisTemplate` is autowired in service classes.

#### 2. **Kafka Integration**
- Message-based communication using Kafka.
- Produces notifications to a topic and sends email alerts.

#### 3. **Log4j2 Integration**
- Enhanced logging using Log4j2 in key methods.

#### 4. **Splunk Integration**
- Centralized logging to Splunk using custom appender configurations.

#### 5. **OAuth2 Integration**
- Secure user authentication and API access in `UserManagement`.

#### 6. **Spring Cloud Gateway**
- API gateway for routing requests with security checks.

#### 7. **Inter-Microservice Communication**
- REST API consumption between `CreditScoringService` and `UserManagement`.

---
