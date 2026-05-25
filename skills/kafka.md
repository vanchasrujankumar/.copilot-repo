# Kafka Skill

## Overview
Expertise in Apache Kafka for building real-time data pipelines and streaming applications.

## Core Concepts

### Architecture
- **Topics**: Categories for messages
- **Partitions**: Ordered, immutable sequences
- **Producers**: Publish messages to topics
- **Consumers**: Read messages from topics
- **Consumer Groups**: Coordinate consumer instances
- **Brokers**: Kafka servers
- **ZooKeeper/KRaft**: Cluster coordination

### Key Concepts
- Offset management
- Consumer groups and rebalancing
- Partition assignment strategies
- Message retention policies

## Producer Configuration

### Core Settings
- `bootstrap.servers`
- `key.serializer`
- `value.serializer`
- `acks` (0, 1, all)
- `retries` and `max.in.flight.requests.per.connection`

### Reliability
- Idempotent producers
- Transactional producers
- Exactly-once semantics

### Performance
- Batch size and linger time
- Compression (snappy, gzip, zstd)
- Buffer memory settings

## Consumer Configuration

### Core Settings
- `bootstrap.servers`
- `key.deserializer`
- `value.deserializer`
- `group.id`
- `auto.offset.reset`

### Reliability
- Manual commit vs. auto commit
- Transactional consumption
- Dead letter queues

### Performance
- Max poll records
- Fetch size settings
- Heartbeat configuration

## Kafka Streams

### Core Concepts
- DSL vs. Processor API
- State stores
- Windowing operations
- Joins (inner, outer, left)

### Common Patterns
- Event time processing
- Windowed aggregations
- Stream-table joins
- KTable changelog streams

## Kafka Connect

### Sources
- Database CDC (Debezium)
- File system sources
- Message queue sources

### Sinks
- Database sinks
- Object storage sinks
- Search engine sinks

### Configuration
- Worker configuration
- Connector configuration
- Transformation (SMTs)

## Schema Registry

- Schema evolution
- Compatibility modes
- Avro/Protobuf/JSON Schema support
- REST API usage

## Monitoring

### Metrics
- Producer/Consumer lag
- Throughput metrics
- Broker metrics
- JVM metrics

### Tools
- Prometheus/JMX exporters
- Grafana dashboards
- Burrow (consumer lag)
- Cruise Control (cluster optimization)

## Security

### Authentication
- SSL/TLS
- SASL/PLAIN
- SASL/SCRAM
- SASL/OAUTHBEARER

### Authorization
- ACLs
- RBAC (Confluent)

## Best Practices

1. Design for at-least-once delivery
2. Use idempotent producers
3. Monitor consumer lag
4. Test with local Kafka
5. Use schema registry for evolution
6. Implement proper error handling
7. Configure appropriate retention
8. Use separate consumer groups for different processing needs
