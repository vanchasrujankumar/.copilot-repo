# DevOps Engineer Skill

## Overview
Expertise in building and maintaining CI/CD pipelines, infrastructure as code, and cloud infrastructure.

## Core Competencies

### CI/CD Pipelines
- **GitHub Actions**: Workflow configuration
- **GitLab CI**: Pipeline definition
- **Jenkins**: Pipeline as code
- **Argo CD**: GitOps deployment
- **Flux**: Kubernetes GitOps

### Infrastructure as Code
- **Terraform**: AWS, Azure, GCP resources
- **CloudFormation**: AWS native
- **Pulumi**: Infrastructure with code
- **Ansible**: Configuration management

### Containerization
- **Docker**: Image creation, multi-stage builds
- **Kubernetes**: Deployments, Services, Ingress
- **Helm**: Package management
- **Kustomize**: Configuration management

### Cloud Platforms
- **AWS**: EC2, S3, RDS, EKS, Lambda
- **Azure**: App Service, AKS, SQL Database
- **GCP**: GKE, Cloud Run, Cloud SQL

## Key Technologies

### Monitoring & Logging
- **Prometheus**: Metrics collection
- **Grafana**: Visualization
- **Loki**: Log aggregation
- **Jaeger/Zipkin**: Distributed tracing
- **ELK Stack**: Elasticsearch, Logstash, Kibana

### Service Mesh
- **Istio**: Traffic management, security
- **Linkerd**: Lightweight service mesh
- **Consul**: Service discovery

### Networking
- **Kubernetes Networking**: Services, Ingress, CNI
- **Load Balancing**: NLB, ALB, HAProxy
- **DNS Management**: Route 53, Cloudflare

## Security Practices

### Container Security
- Image scanning (Trivy, Snyk)
- Minimal base images
- Non-root containers
- Secret management (Vault, AWS Secrets Manager)

### Infrastructure Security
- IAM best practices
- Network segmentation
- Encryption at rest and in transit
- Security scanning in pipelines

### Compliance
- CIS benchmarks
- SOC2, ISO 27001
- GDPR considerations

## Automation Patterns

### Infrastructure Provisioning
- Terraform modules
- Reusable components
- State management
- Backend configuration

### Deployment Strategies
- Blue-green deployments
- Canary releases
- Rolling updates
- Feature flags

### GitOps
- Declarative infrastructure
- Git as source of truth
- Automated sync
- Drift detection

## Best Practices

1. **Infrastructure as Code**
   - Version all infrastructure
   - Use modules for reusability
   - Test infrastructure changes
   - Implement state locking

2. **CI/CD Best Practices**
   - Fast feedback loops
   - Parallel test execution
   - Automated rollback
   - Build once, deploy many

3. **Monitoring & Alerting**
   - Define SLIs/SLOs
   - Alert on symptoms, not causes
   - Use dashboards for visibility
   - Implement runbooks

4. **Security**
   - Scan for vulnerabilities
   - Use least privilege
   - Encrypt sensitive data
   - Regular security audits

5. **Reliability**
   - Design for failure
   - Implement circuit breakers
   - Use health checks
   - Regular disaster recovery tests

## Common Workflows

### Deploying to Kubernetes
1. Build Docker image
2. Push to registry
3. Update deployment manifest
4. Apply with kubectl or Helm
5. Verify deployment
6. Monitor for issues

### Infrastructure Changes
1. Update Terraform code
2. Run `terraform plan`
3. Review changes
4. Apply in staging
5. Test in staging
6. Apply in production

## Tools & Technologies

- **Kubernetes**: Orchestration
- **Docker**: Containerization
- **Terraform**: IaC
- **Prometheus**: Monitoring
- **Grafana**: Visualization
- **Helm**: Package management
- **Argo CD**: GitOps
- **Vault**: Secrets management
