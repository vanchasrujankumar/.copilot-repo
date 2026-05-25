# Grafana Skill

## Overview
Expertise in Grafana for monitoring, visualization, and observability dashboards.

## Core Concepts

### Architecture
- **Dashboards**: Visual representations of metrics
- **Panels**: Individual visualizations (graph, gauge, table, etc.)
- **Data Sources**: Connections to metrics backends
- **Alerts**: Threshold-based notifications
- **Annotations**: Event markers on graphs

### Data Sources
- Prometheus
- InfluxDB
- Elasticsearch
- Graphite
- MySQL/PostgreSQL
- CloudWatch
- Loki (logs)
- Tempo (traces)

## Dashboard Design

### Best Practices
- Clear, actionable visualizations
- Consistent color schemes
- Appropriate time ranges
- Contextual annotations
- Drill-down capabilities

### Panel Types
- **Graph**: Time series visualization
- **Gauge**: Single value with thresholds
- **Table**: Tabular data display
- **Stat**: Large single value
- **Heatmap**: Distribution visualization
- **Logs**: Log exploration
- **State timeline**: State changes over time

## Querying Data

### PromQL (Prometheus)
- Rate and irate functions
- Aggregation operators
- Vector matching
- Recording rules

### InfluxQL/Flux
- SELECT statements
- Aggregations
- Window functions
- Flux for complex queries

### Elasticsearch Query
- DSL queries
- Aggregations
- Scripted fields

## Alerting

### Alert Rules
- Threshold-based alerts
- Expression evaluation
- For duration configuration

### Notification Channels
- Email
- Slack
- PagerDuty
- Webhook
- OpsGenie
- VictorOps

### Alert States
- Normal
- Pending
- Firing

## Templating

### Variables
- Query-based variables
- Custom variables
- Variable interpolation
- Dynamic dashboard customization

## Data Source Configuration

### Prometheus
- Job discovery
- Service discovery
- Relabeling rules

### InfluxDB
- Database selection
- Retention policies
- Flux script configuration

### Elasticsearch
- Index patterns
- Time field configuration
- Query mode (legacy vs. Lucene)

## Security

### Authentication
- Basic auth
- LDAP
- OAuth (GitHub, GitLab, Google)
- SAML

### Authorization
- Organization roles
- Dashboard permissions
- Folder permissions

## Best Practices

1. Use consistent naming conventions
2. Document dashboard purpose
3. Set appropriate alert thresholds
4. Use folders for organization
5. Implement dashboard versioning
6. Create reusable panels
7. Monitor Grafana itself
8. Use annotations for deployments
