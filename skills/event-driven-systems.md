# Event-Driven Systems Skill

## Overview
Expertise in designing, implementing, and maintaining event-driven architectures using modern technologies.

## Core Concepts

### Event-Driven Architecture (EDA)
- Event sourcing pattern
- CQRS (Command Query Responsibility Segregation)
- Eventual consistency patterns
- Dead letter queues and retry mechanisms

### Technologies
- **Kafka**: Topics, partitions, consumers, producers, consumer groups
- **AWS EventBridge**: Rules, patterns, targets
- **RabbitMQ**: Exchanges, queues, bindings
- **Pub/Sub**: Subscriptions, topics, message ordering

### Best Practices
- Idempotent event processing
- Event versioning strategies
- Schema evolution with Avro/Protobuf
- Backpressure handling
- Circuit breakers for event processing

## Common Patterns

### Saga Pattern
- Orchestration-based sagas
- Choreography-based sagas
- Compensation transactions

### Outbox Pattern
- Database transaction + message outbox
- Change data capture (CDC)
- Debezium integration

### Retry & Dead Letter
- Exponential backoff
- Retry policies
- DLQ configuration

## Implementation Guidelines

1. Design events as nouns in past tense
2. Include correlation IDs for tracing
3. Use structured schemas for events
4. Implement idempotency keys
5. Monitor event processing lag

## Testing Strategies

- Event-driven unit tests
- Contract testing with Pact
- Integration tests with test containers
- Load testing with k6 or Gatling

## Monitoring & Observability

- Event throughput metrics
- Processing lag monitoring
- Dead letter queue alerts
- Distributed tracing with OpenTelemetry
