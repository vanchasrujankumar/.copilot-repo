# Java Microservices Skill

## Overview
Expertise in building scalable, resilient Java microservices with Spring Boot and related technologies.

## Core Technologies

### Spring Framework
- Spring Boot auto-configuration
- Spring Cloud (Config, Discovery, Gateway)
- Spring Security (OAuth2, JWT)
- Spring Data JPA, MongoDB, Redis
- Spring WebFlux (reactive programming)

### Service Communication
- RESTful APIs with OpenAPI/Swagger
- gRPC for internal services
- Feign clients for declarative REST
- Service discovery with Eureka/Nacos

### Resilience Patterns
- Circuit breaker (Resilience4j/Hystrix)
- Retry policies
- Bulkhead isolation
- Timeout handling

## Architecture Patterns

### Microservice Design
- Bounded contexts
- Domain-driven design (DDD)
- Hexagonal/Clean architecture
- Ports and adapters pattern

### Database Patterns
- Database per service
- CQRS pattern
- Outbox pattern for events
- Polyglot persistence

## Configuration & Deployment

### Configuration Management
- Externalized configuration
- Spring Cloud Config
- Profile-specific configs
- Secrets management

### Containerization
- Docker best practices
- Multi-stage builds
- Health checks
- Resource limits

### Kubernetes
- Deployments, Services, Ingress
- ConfigMaps, Secrets
- Horizontal Pod Autoscaler
- Service Mesh (Istio/Linkerd)

## Testing Strategies

### Unit Testing
- JUnit 5 with Mockito
- Testcontainers for integration
- Spring Boot Test slices

### Contract Testing
- Pact for consumer-driven contracts
- Spring Cloud Contract

### Performance Testing
- JMeter for load testing
- Micrometer metrics

## Monitoring & Observability

- Spring Boot Actuator endpoints
- Micrometer with Prometheus/Grafana
- Distributed tracing with Zipkin/Jaeger
- Health checks and readiness probes

## Security Best Practices

- OAuth2 resource server configuration
- JWT validation
- CORS configuration
- Rate limiting
- Input validation
