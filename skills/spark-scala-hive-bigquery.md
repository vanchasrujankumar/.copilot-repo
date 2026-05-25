# Spark, Scala, Hive, BigQuery Skill

## Overview
Expertise in big data processing with Apache Spark, Scala, Hive, and Google BigQuery.

## Apache Spark

### Core Concepts
- **RDD**: Resilient Distributed Dataset (immutable)
- **DataFrame**: Distributed collection with schema
- **Dataset**: Typed version of DataFrame
- **SparkSession**: Entry point for Spark functionality

### Programming Models
- **Batch Processing**: Static data processing
- **Structured Streaming**: Stream processing with DataFrame API
- **Spark SQL**: SQL queries on structured data

### Transformations
- `map`, `filter`, `flatMap`
- `groupByKey`, `reduceByKey`
- `join`, `union`, `distinct`
- `agg`, `groupBy`, `sort`

### Actions
- `collect`, `count`, `first`
- `take`, `saveAsTextFile`
- `foreach`, `foreachPartition`

### Performance Optimization
- **Caching**: `persist()`, `cache()`
- **Partitioning**: Optimal partition count
- **Serialization**: Kryo serialization
- **Broadcast Variables**: Small dataset distribution
- **Accumulators**: Distributed counters

## Scala

### Functional Programming
- Immutable collections
- Higher-order functions
- Pattern matching
- Case classes

### Collections
- `List`, `Set`, `Map`
- `Vector`, `Array`
- `Option`, `Either`
- Stream processing with `map`, `filter`, `fold`

### Concurrency
- Futures and Promises
- Akka actors (optional)
- Parallel collections

### Best Practices
- Prefer immutable data structures
- Use pattern matching for complex logic
- Leverage for-comprehensions
- Handle `Option` properly

## Apache Hive

### Core Concepts
- **HiveQL**: SQL-like query language
- **Metastore**: Metadata repository
- **Hive Server**: Query execution engine
- **Tez/Spark Engine**: Execution engines

### Data Types
- Primitive types (INT, STRING, BOOLEAN)
- Complex types (ARRAY, MAP, STRUCT)
- Partitioning columns

### Table Types
- **Managed Tables**: Hive manages data lifecycle
- **External Tables**: Point to external data
- **Partitioned Tables**: Partitioned by columns
- **Bucketed Tables**: Bucketed for efficient joins

### Optimization
- **Partition Pruning**: Filter partitions
- **Bucketing**: Efficient joins
- **Vectorized Query Execution**
- **Cost-Based Optimization (CBO)**
- **ORC/Parquet formats**

## Google BigQuery

### Core Concepts
- **Tables**: Data storage units
- **Views**: Saved queries
- **Materialized Views**: Pre-computed results
- **Data Transfer**: Ingestion services

### Query Language
- Standard SQL (recommended)
- Legacy SQL (deprecated)
- Window functions
- Array and struct operations

### Performance Optimization
- **Partitioning**: Date/time partitioning
- **Clustering**: Column-based clustering
- **Materialized Views**: Pre-aggregation
- **Query Caching**: Automatic caching

### Data Ingestion
- **Batch**: Load from Cloud Storage
- **Streaming**: InsertAll API
- **Data Transfer**: Automated ingestion
- **Change Data Capture**: With BigQuery Change Data Capture

### Best Practices
1. Use partitioned and clustered tables
2. Avoid `SELECT *` in production
3. Use `LIMIT` during development
4. Leverage materialized views
5. Monitor query costs
6. Use `EXCEPT` for schema evolution
7. Partition large tables
8. Use streaming inserts sparingly

## Integration Patterns

### Spark + Hive
- Hive Metastore integration
- Read/write Hive tables
- Hive UDFs in Spark

### Spark + BigQuery
- BigQuery connector for Spark
- Read/write BigQuery tables
- Pushdown predicates

### ETL Patterns
- Extract from source systems
- Transform with Spark
- Load to data warehouse
- Validate with assertions

## Testing Strategies

### Unit Testing
- Spark Test Suite
- ScalaTest for business logic
- Mock data generation

### Integration Testing
- Testcontainers for Spark
- Local BigQuery emulator
- MiniCluster for Hive

### Performance Testing
- Query execution time
- Resource utilization
- Data skew detection
