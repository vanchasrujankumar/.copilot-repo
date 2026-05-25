# Java Architect Skill

## Overview
Expertise in designing scalable, maintainable Java enterprise applications and microservices.

## Core Competencies

### Architecture Design
- **Domain-Driven Design (DDD)**: Bounded contexts, aggregates, domain events
- **Clean Architecture**: Separation of concerns, dependency inversion
- **Hexagonal Architecture**: Ports and adapters pattern
- **CQRS**: Command Query Responsibility Segregation
- **Event Sourcing**: State as sequence of events

### Technology Stack
- **Spring Framework**: Boot, Cloud, Security, Data
- **Microservices**: Service discovery, config, gateway
- **API Design**: REST, GraphQL, gRPC
- **Build Tools**: Maven, Gradle

### Patterns & Best Practices
- **Design Patterns**: Factory, Strategy, Observer, Decorator
- **Anti-Patterns**: God objects, tight coupling, premature optimization
- **SOLID Principles**: Single responsibility, open/closed, Liskov substitution, interface segregation, dependency inversion

## System Design

### Scalability
- Horizontal vs. vertical scaling
- Load balancing strategies
- Caching strategies (CDN, Redis)
- Database sharding and replication

### Resilience
- Circuit breakers (Resilience4j)
- Retry policies
- Bulkhead isolation
- Timeout handling
- Fallback mechanisms

### Security
- OAuth2 and OpenID Connect
- JWT token management
- Role-based access control
- API security best practices
- Secret management

## Data Architecture

### Database Design
- Relational (PostgreSQL, MySQL)
- NoSQL (MongoDB, Cassandra)
- Polyglot persistence
- Database migration (Flyway, Liquibase)

### Event-Driven Architecture
- Kafka for messaging
- Event sourcing patterns
- CDC with Debezium
- Eventual consistency

## Cloud Architecture

### AWS Services
- EC2, ECS, EKS
- RDS, DynamoDB
- S3, CloudFront
- Lambda, API Gateway
- CloudWatch, CloudTrail

### Azure Services
- Azure App Service
- Azure Kubernetes Service
- Azure SQL Database
- Azure Cosmos DB
- Azure Functions

### GCP Services
- Google Kubernetes Engine
- Cloud Run
- Cloud SQL
- BigQuery
- Cloud Storage

## Monitoring & Observability

### Logging
- Structured logging
- Log aggregation (ELK, Loki)
- Correlation IDs
- Log levels and filtering

### Metrics
- Micrometer with Prometheus
- Custom metrics
- Business metrics
- Alerting on metrics

### Tracing
- Distributed tracing
- OpenTelemetry
- Jaeger, Zipkin
- Trace context propagation

## DevOps & SRE

### CI/CD
- Pipeline as code
- Automated testing
- Blue-green deployments
- Canary releases

### Infrastructure as Code
- Terraform
- AWS CloudFormation
- Azure Resource Manager
- Helm charts

### SRE Practices
- SLIs, SLOs, SLAs
- Error budget management
- Incident response
- Post-mortem culture

## Best Practices

1. Design for testability
2. Prefer composition over inheritance
3. Use immutable objects
4. Implement proper error handling
5. Document architecture decisions (ADRs)
6. Code for maintainability
7. Optimize for change
8. Monitor everything
9. Automate everything
10. Plan for failure
