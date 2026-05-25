# Vela Skill

## Overview
Expertise in Vela (Open Application Model) for defining and managing cloud-native applications.

## Core Concepts

### OAM (Open Application Model)
- **Components**: Deployable units (containers, functions)
- **Traits**: Runtime behaviors (scaling, ingress, auto-scaling)
- **Scopes**: Environmental contexts (namespaces, networks)
- **Workloads**: Abstracted deployment targets

### Architecture
- **Application**: Bundle of components + traits + scopes
- **Application Configuration**: Runtime-specific settings
- **Definition**: Reusable component/trait/scope templates

## Component Types

### Container Workload
- Image specification
- Resource requests/limits
- Environment variables
- Command/args overrides

### Function Workload
- Function definition
- Trigger configuration
- Runtime environment

### Sidecar Pattern
- Sidecar containers
- Shared volumes
- Network configuration

## Traits

### Scaling Traits
- **Scaler**: Horizontal pod autoscaling
- **Ingress**: HTTP routing configuration
- **Task**: Cron job scheduling

### Observability Traits
- **Monitor**: Metrics collection
- **Log**: Log aggregation
- **Status**: Application status reporting

### Security Traits
- **Secret**: Secret injection
- **NetworkPolicy**: Network restrictions
- **RBAC**: Role-based access control

### Deployment Traits
- **Rollout**: Deployment strategy
- **HealthCheck**: Liveness/readiness probes
- **Affinity**: Pod scheduling rules

## Scopes

### Network Scope
- Service mesh integration
- Ingress configuration
- Service discovery

### Storage Scope
- Persistent volume claims
- Storage class selection
- Volume snapshots

### Environment Scope
- Namespace isolation
- Resource quotas
- Limit ranges

## Application Definition

### Component Definition
- Schema definition
- Required properties
- Trait compatibility

### Trait Definition
- Schema definition
- Apply to workloads
- Configuration options

## KubeVela Integration

### CLI Commands
- `vela init`: Initialize OAM environment
- `vela up`: Deploy application
- `vela status`: Check application status
- `vela logs`: View application logs
- `vela ls`: List applications

### Workflow
- Deploy application with `vela up`
- Update configuration
- Rollback to previous version
- Scale components

## Best Practices

1. Define components as reusable templates
2. Use traits for environment-specific configurations
3. Separate application definition from configuration
4. Implement health checks as traits
5. Use scopes for cross-cutting concerns
6. Version application definitions
7. Test in staging before production
8. Monitor application health

## CI/CD Integration

### GitOps
- Application manifests in Git
- ArgoCD integration
- Flux integration

### Pipeline
- Build and push images
- Update application configuration
- Deploy with `vela up`
- Verify deployment
