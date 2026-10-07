# SRE / DevOps / Cloud Platform --- 3-Month Master Checklist

**Target niche:** SRE / Cloud Platform Engineer --- AWS \| Kubernetes \|
Terraform \| CI/CD \| Python Automation \| Observability

**Goal:** Cover the KNIME Senior SRE-style JD end-to-end, while building
practical interview and production-troubleshooting capability.

------------------------------------------------------------------------

## 1. AWS / Cloud Engineering

### AWS Fundamentals

-   [ ] AWS global infrastructure: Regions, Availability Zones, edge
    locations
-   [ ] Shared Responsibility Model
-   [ ] AWS account structure and environments
-   [ ] IAM users, groups, roles and policies
-   [ ] Least privilege
-   [ ] AWS CLI basics
-   [ ] AWS SDK / boto3 basics
-   [ ] AWS pricing fundamentals

### VPC & Networking

-   [ ] VPC architecture
-   [ ] CIDR and subnetting
-   [ ] Public vs private subnets
-   [ ] Route tables
-   [ ] Internet Gateway
-   [ ] NAT Gateway
-   [ ] Security Groups
-   [ ] Network ACLs
-   [ ] DNS / Route 53 fundamentals
-   [ ] VPC endpoints
-   [ ] VPC peering
-   [ ] Transit Gateway concepts
-   [ ] Load Balancers
-   [ ] ALB vs NLB
-   [ ] Target groups
-   [ ] Health checks
-   [ ] TLS termination
-   [ ] Common network troubleshooting

### EC2

-   [ ] Instance types
-   [ ] AMI
-   [ ] EBS
-   [ ] Instance lifecycle
-   [ ] User data
-   [ ] IAM roles for EC2
-   [ ] Auto Scaling Groups
-   [ ] Launch templates
-   [ ] CloudWatch metrics
-   [ ] EC2 troubleshooting
-   [ ] CPU / memory / disk / network analysis

### S3

-   [ ] Buckets and objects
-   [ ] Bucket policies
-   [ ] IAM access
-   [ ] Versioning
-   [ ] Lifecycle policies
-   [ ] Encryption
-   [ ] Storage classes
-   [ ] Cross-region replication concepts
-   [ ] Troubleshoot AccessDenied

### IAM

-   [ ] Users vs roles
-   [ ] Managed vs inline policies
-   [ ] Policy evaluation logic
-   [ ] Resource-based policies
-   [ ] AssumeRole
-   [ ] Trust policies
-   [ ] STS
-   [ ] Cross-account access
-   [ ] Troubleshoot AccessDenied

### RDS / PostgreSQL

-   [ ] RDS fundamentals
-   [ ] PostgreSQL basics
-   [ ] Connection strings
-   [ ] Security groups
-   [ ] Parameter groups
-   [ ] Backups
-   [ ] Multi-AZ
-   [ ] Read replicas
-   [ ] Connection limits
-   [ ] Connection pool concepts
-   [ ] CPU / memory / storage / connection troubleshooting

### ECR

-   [ ] Container repositories
-   [ ] Image tagging
-   [ ] Image push / pull
-   [ ] IAM permissions
-   [ ] Image scanning
-   [ ] Lifecycle policies
-   [ ] ECR integration with EKS

### CloudWatch

-   [ ] Metrics
-   [ ] Logs
-   [ ] Alarms
-   [ ] Dashboards
-   [ ] Log Insights
-   [ ] EC2 monitoring
-   [ ] RDS monitoring
-   [ ] EKS monitoring
-   [ ] Application health monitoring

------------------------------------------------------------------------

# 2. Kubernetes / EKS

## Kubernetes Architecture

-   [ ] Control plane
-   [ ] API Server
-   [ ] etcd
-   [ ] Scheduler
-   [ ] Controller Manager
-   [ ] Kubelet
-   [ ] Kube-proxy
-   [ ] Container runtime
-   [ ] Kubernetes API flow
-   [ ] Desired vs actual state
-   [ ] Controllers / reconciliation

## Kubernetes Objects

-   [ ] Namespace
-   [ ] Pod
-   [ ] ReplicaSet
-   [ ] Deployment
-   [ ] StatefulSet
-   [ ] DaemonSet
-   [ ] Job
-   [ ] CronJob
-   [ ] Service
-   [ ] ConfigMap
-   [ ] Secret
-   [ ] PersistentVolume
-   [ ] PersistentVolumeClaim
-   [ ] StorageClass
-   [ ] Ingress
-   [ ] ServiceAccount
-   [ ] Role
-   [ ] RoleBinding
-   [ ] ClusterRole
-   [ ] ClusterRoleBinding

## Kubernetes Workloads

-   [ ] Deployment strategies
-   [ ] Rolling update
-   [ ] Recreate
-   [ ] Rollout history
-   [ ] Rollback
-   [ ] Stateful applications
-   [ ] Daemon workloads
-   [ ] Batch workloads

## Kubernetes Networking

-   [ ] Pod networking
-   [ ] Service networking
-   [ ] ClusterIP
-   [ ] NodePort
-   [ ] LoadBalancer
-   [ ] Ingress
-   [ ] DNS / CoreDNS
-   [ ] NetworkPolicy
-   [ ] Kubernetes-to-AWS networking
-   [ ] AWS Load Balancer Controller
-   [ ] ALB / NLB integration

## Configuration

-   [ ] ConfigMaps
-   [ ] Secrets
-   [ ] Environment variables
-   [ ] Secret injection
-   [ ] Mounted configuration
-   [ ] Configuration versioning

## Health & Reliability

-   [ ] Liveness probes
-   [ ] Readiness probes
-   [ ] Startup probes
-   [ ] Graceful shutdown
-   [ ] terminationGracePeriodSeconds
-   [ ] PodDisruptionBudget
-   [ ] Replica management
-   [ ] Anti-affinity
-   [ ] Topology spread constraints

## Resources

-   [ ] CPU requests
-   [ ] CPU limits
-   [ ] Memory requests
-   [ ] Memory limits
-   [ ] QoS classes
-   [ ] OOMKilled
-   [ ] ResourceQuota
-   [ ] LimitRange

## Scheduling

-   [ ] Node selectors
-   [ ] Affinity
-   [ ] Anti-affinity
-   [ ] Taints
-   [ ] Tolerations
-   [ ] Pod priority
-   [ ] Scheduling failures

## Scaling

-   [ ] Horizontal Pod Autoscaler
-   [ ] Vertical Pod Autoscaler concepts
-   [ ] Cluster Autoscaler
-   [ ] Karpenter concepts
-   [ ] CPU-based scaling
-   [ ] Memory-based scaling
-   [ ] Custom metrics

## EKS

-   [ ] EKS architecture
-   [ ] Managed node groups
-   [ ] Fargate concepts
-   [ ] EKS IAM
-   [ ] IRSA / Pod Identity concepts
-   [ ] EKS networking
-   [ ] AWS Load Balancer Controller
-   [ ] EKS upgrades
-   [ ] EKS troubleshooting
-   [ ] EKS observability
-   [ ] EKS cost considerations

------------------------------------------------------------------------

# 3. Kubernetes Troubleshooting

Practice each scenario until you can explain:

**Symptom → Evidence → Investigation → Root Cause → Mitigation →
Permanent Fix → Prevention**

-   [ ] Pod Pending
-   [ ] Pod CrashLoopBackOff
-   [ ] Pod ImagePullBackOff
-   [ ] Pod OOMKilled
-   [ ] Pod constantly restarting
-   [ ] Readiness probe failing
-   [ ] Liveness probe failing
-   [ ] Deployment stuck
-   [ ] Rollout failure
-   [ ] Service unreachable
-   [ ] Ingress returning 404
-   [ ] Ingress returning 502
-   [ ] Ingress returning 503
-   [ ] DNS resolution failure
-   [ ] CoreDNS issue
-   [ ] NetworkPolicy blocking traffic
-   [ ] Pod cannot connect to database
-   [ ] High CPU
-   [ ] High memory
-   [ ] Disk pressure
-   [ ] Node NotReady
-   [ ] Scheduling failure
-   [ ] Certificate expiry
-   [ ] Secret/configuration issue
-   [ ] Image vulnerability
-   [ ] Application latency
-   [ ] Intermittent connectivity
-   [ ] Deployment caused production degradation

## Essential kubectl

-   [ ] `kubectl get`
-   [ ] `kubectl describe`
-   [ ] `kubectl logs`
-   [ ] `kubectl exec`
-   [ ] `kubectl top`
-   [ ] `kubectl rollout`
-   [ ] `kubectl scale`
-   [ ] `kubectl apply`
-   [ ] `kubectl delete`
-   [ ] `kubectl explain`
-   [ ] `kubectl get events`
-   [ ] JSONPath
-   [ ] Label selectors
-   [ ] Field selectors
-   [ ] Debug containers / ephemeral containers concepts

------------------------------------------------------------------------

# 4. Helm

-   [ ] Helm architecture
-   [ ] Charts
-   [ ] Templates
-   [ ] `values.yaml`
-   [ ] Template functions
-   [ ] Release lifecycle
-   [ ] Install
-   [ ] Upgrade
-   [ ] Rollback
-   [ ] Uninstall
-   [ ] Helm repositories
-   [ ] Chart dependencies
-   [ ] Environment-specific values
-   [ ] Helm secrets concepts
-   [ ] Helm troubleshooting
-   [ ] Helm linting
-   [ ] Helm in CI/CD
-   [ ] Helm with Argo CD

------------------------------------------------------------------------

# 5. Kubernetes Operators

-   [ ] Operator pattern
-   [ ] Custom Resource Definition (CRD)
-   [ ] Custom Resources (CR)
-   [ ] Controllers
-   [ ] Reconciliation loop
-   [ ] Operator lifecycle
-   [ ] Operator troubleshooting
-   [ ] Understand why operators are useful for stateful/platform
    workloads
-   [ ] Basic hands-on with an existing operator
-   [ ] Understand Operator SDK concepts

------------------------------------------------------------------------

# 6. Infrastructure as Code

## Terraform

-   [ ] Terraform architecture
-   [ ] Providers
-   [ ] Resources
-   [ ] Data sources
-   [ ] Variables
-   [ ] Outputs
-   [ ] Locals
-   [ ] Modules
-   [ ] State
-   [ ] Remote state
-   [ ] State locking
-   [ ] `terraform init`
-   [ ] `terraform plan`
-   [ ] `terraform apply`
-   [ ] `terraform destroy`
-   [ ] Import
-   [ ] State manipulation
-   [ ] Drift
-   [ ] Workspaces
-   [ ] Environment separation
-   [ ] Secrets handling
-   [ ] Terraform formatting
-   [ ] Terraform validation
-   [ ] Terraform linting
-   [ ] Terraform security scanning
-   [ ] Terraform CI/CD
-   [ ] Reusable modules

### Terraform Project

-   [ ] VPC
-   [ ] Subnets
-   [ ] Route tables
-   [ ] Security groups
-   [ ] IAM
-   [ ] ECR
-   [ ] EKS
-   [ ] RDS
-   [ ] CloudWatch

## CloudFormation

-   [ ] CloudFormation basics
-   [ ] Templates
-   [ ] Parameters
-   [ ] Outputs
-   [ ] Resources
-   [ ] Stack lifecycle
-   [ ] Nested stacks
-   [ ] Change sets
-   [ ] Terraform vs CloudFormation

------------------------------------------------------------------------

# 7. Azure

The goal is **working knowledge**, not replacing AWS as the primary
specialization.

## Azure Fundamentals

-   [ ] Azure Regions
-   [ ] Availability Zones
-   [ ] Resource Groups
-   [ ] Subscriptions
-   [ ] Management Groups
-   [ ] Azure Portal
-   [ ] Azure CLI
-   [ ] Azure Cloud Shell

## Azure Networking

-   [ ] Virtual Network
-   [ ] Subnets
-   [ ] NSG
-   [ ] Route tables
-   [ ] Public IP
-   [ ] Private endpoints
-   [ ] Load Balancer
-   [ ] Application Gateway
-   [ ] Azure DNS
-   [ ] VPN concepts

## Azure Identity

-   [ ] Microsoft Entra ID
-   [ ] Service principals
-   [ ] Managed identities
-   [ ] RBAC
-   [ ] Conditional access concepts
-   [ ] Key Vault

## Azure Compute

-   [ ] Virtual Machines
-   [ ] VM Scale Sets
-   [ ] AKS
-   [ ] Container Registry
-   [ ] Azure Container Instances concepts

## Azure Storage

-   [ ] Blob Storage
-   [ ] Files
-   [ ] Storage Accounts
-   [ ] Storage tiers
-   [ ] Lifecycle management

## Azure Database

-   [ ] Azure Database for PostgreSQL
-   [ ] Connection/security basics
-   [ ] Backup / HA concepts

## Azure Monitoring

-   [ ] Azure Monitor
-   [ ] Log Analytics
-   [ ] Application Insights
-   [ ] Alerts
-   [ ] Dashboards

## AWS → Azure Mapping

-   [ ] VPC → VNet
-   [ ] IAM → Entra ID / RBAC
-   [ ] EC2 → Azure VM
-   [ ] EKS → AKS
-   [ ] ECR → ACR
-   [ ] S3 → Blob Storage
-   [ ] CloudWatch → Azure Monitor
-   [ ] RDS → Azure Database
-   [ ] ALB → Application Gateway / Load Balancer

------------------------------------------------------------------------

# 8. CI/CD & Release Engineering

## Jenkins

-   [ ] Jenkins architecture
-   [ ] Controller
-   [ ] Agents
-   [ ] Static agents
-   [ ] Dynamic agents
-   [ ] Pipeline
-   [ ] Declarative pipeline
-   [ ] Scripted pipeline concepts
-   [ ] Jenkinsfile
-   [ ] Parameters
-   [ ] Credentials
-   [ ] Secrets
-   [ ] Environment variables
-   [ ] Build triggers
-   [ ] Webhooks
-   [ ] Artifacts
-   [ ] Workspace
-   [ ] Pipeline stages
-   [ ] Parallel stages
-   [ ] Retry / timeout
-   [ ] Approval gates
-   [ ] Rollback
-   [ ] Pipeline failure troubleshooting

## Self-Hosted Runners / Agents

-   [ ] Why self-hosted runners are used
-   [ ] Agent registration
-   [ ] Labels
-   [ ] Executor concepts
-   [ ] Docker-based agents
-   [ ] Kubernetes-based agents
-   [ ] Agent capacity
-   [ ] Disk cleanup
-   [ ] Agent connectivity troubleshooting
-   [ ] Credential/security considerations

## Git

-   [ ] Clone
-   [ ] Branch
-   [ ] Commit
-   [ ] Push
-   [ ] Pull
-   [ ] Merge
-   [ ] Rebase
-   [ ] Cherry-pick
-   [ ] Revert
-   [ ] Reset
-   [ ] Tags
-   [ ] Pull requests
-   [ ] Branching strategies
-   [ ] Git troubleshooting

## Argo CD / GitOps

-   [ ] GitOps principles
-   [ ] Argo CD architecture
-   [ ] Application
-   [ ] ApplicationSet concepts
-   [ ] Sync
-   [ ] Auto-sync
-   [ ] Health status
-   [ ] Drift detection
-   [ ] Rollback
-   [ ] Repository credentials
-   [ ] Argo CD troubleshooting

------------------------------------------------------------------------

# 9. Docker

-   [ ] Images
-   [ ] Containers
-   [ ] Dockerfile
-   [ ] Build context
-   [ ] Layers
-   [ ] Multi-stage builds
-   [ ] Environment variables
-   [ ] Volumes
-   [ ] Networks
-   [ ] Port mapping
-   [ ] Docker Compose
-   [ ] Image tagging
-   [ ] Registry
-   [ ] Image scanning
-   [ ] Container logs
-   [ ] Container resource limits
-   [ ] Docker troubleshooting
-   [ ] Container security

------------------------------------------------------------------------

# 10. Python for SRE / DevOps

## Python Fundamentals

-   [ ] Variables
-   [ ] Data types
-   [ ] Strings
-   [ ] Lists
-   [ ] Tuples
-   [ ] Sets
-   [ ] Dictionaries
-   [ ] Loops
-   [ ] Conditions
-   [ ] Functions
-   [ ] Arguments
-   [ ] Exceptions
-   [ ] Modules
-   [ ] Packages
-   [ ] Virtual environments
-   [ ] File handling
-   [ ] JSON
-   [ ] YAML
-   [ ] Regular expressions
-   [ ] Logging

## Automation

-   [ ] `os`
-   [ ] `sys`
-   [ ] `subprocess`
-   [ ] `pathlib`
-   [ ] `shutil`
-   [ ] `datetime`
-   [ ] `argparse`
-   [ ] `logging`
-   [ ] HTTP requests
-   [ ] REST APIs
-   [ ] Retry logic
-   [ ] Timeout handling
-   [ ] Error handling

## AWS Automation

-   [ ] boto3
-   [ ] EC2 automation
-   [ ] S3 automation
-   [ ] CloudWatch automation
-   [ ] IAM inspection
-   [ ] EKS automation
-   [ ] Cost-reporting script

## Kubernetes Automation

-   [ ] Kubernetes Python client
-   [ ] Pod health checker
-   [ ] Deployment validator
-   [ ] Failed-pod report
-   [ ] Resource report
-   [ ] Namespace health report
-   [ ] Kubernetes event analyzer

## SRE Python Projects

-   [ ] Production-style log analyzer
-   [ ] Linux health-check script
-   [ ] AWS resource checker
-   [ ] Kubernetes diagnostics tool
-   [ ] Deployment validation tool
-   [ ] Certificate expiry checker
-   [ ] API health checker
-   [ ] Disk cleanup automation

------------------------------------------------------------------------

# 11. Bash / Shell

-   [ ] Variables
-   [ ] Conditions
-   [ ] Loops
-   [ ] Functions
-   [ ] Exit codes
-   [ ] `$?`
-   [ ] Arguments
-   [ ] Pipes
-   [ ] Redirection
-   [ ] `grep`
-   [ ] `awk`
-   [ ] `sed`
-   [ ] `cut`
-   [ ] `sort`
-   [ ] `uniq`
-   [ ] `xargs`
-   [ ] `find`
-   [ ] `curl`
-   [ ] `wget`
-   [ ] `jq`
-   [ ] `ps`
-   [ ] `top`
-   [ ] `vmstat`
-   [ ] `iostat`
-   [ ] `free`
-   [ ] `df`
-   [ ] `du`
-   [ ] `ss`
-   [ ] `netstat`
-   [ ] `lsof`
-   [ ] `systemctl`
-   [ ] `journalctl`
-   [ ] Cron
-   [ ] Log rotation
-   [ ] Shell error handling
-   [ ] Production-safe scripting

------------------------------------------------------------------------

# 12. Linux Systems Engineering

## Linux Fundamentals

-   [ ] Filesystem hierarchy
-   [ ] Processes
-   [ ] Threads
-   [ ] Services
-   [ ] Systemd
-   [ ] Permissions
-   [ ] Ownership
-   [ ] Users / groups
-   [ ] Environment variables
-   [ ] Package management
-   [ ] SSH
-   [ ] Logs

## Linux Performance

-   [ ] CPU utilization
-   [ ] Load average
-   [ ] Memory utilization
-   [ ] Swap
-   [ ] Disk utilization
-   [ ] I/O wait
-   [ ] Network utilization
-   [ ] Process investigation
-   [ ] Zombie processes
-   [ ] File descriptors
-   [ ] Connection limits

## Linux Troubleshooting

-   [ ] High CPU
-   [ ] High memory
-   [ ] Disk full
-   [ ] Disk inode exhaustion
-   [ ] High I/O
-   [ ] Process hanging
-   [ ] Service down
-   [ ] Port unavailable
-   [ ] SSH failure
-   [ ] DNS failure
-   [ ] Network connectivity issue

------------------------------------------------------------------------

# 13. Linux Networking

-   [ ] OSI model
-   [ ] TCP/IP
-   [ ] TCP handshake
-   [ ] UDP
-   [ ] Ports
-   [ ] Sockets
-   [ ] DNS
-   [ ] HTTP
-   [ ] HTTPS
-   [ ] TLS
-   [ ] Certificates
-   [ ] Routing
-   [ ] NAT
-   [ ] Firewall
-   [ ] Proxy
-   [ ] Load balancing
-   [ ] Connection timeout
-   [ ] Connection refused
-   [ ] Connection reset
-   [ ] DNS timeout
-   [ ] Packet loss
-   [ ] Latency

## Commands

-   [ ] `ping`
-   [ ] `curl`
-   [ ] `dig`
-   [ ] `nslookup`
-   [ ] `traceroute`
-   [ ] `ss`
-   [ ] `tcpdump`
-   [ ] `nc`
-   [ ] `openssl s_client`

------------------------------------------------------------------------

# 14. Load Balancing

-   [ ] Layer 4 vs Layer 7
-   [ ] Round robin
-   [ ] Weighted routing
-   [ ] Least connections
-   [ ] Health checks
-   [ ] Connection draining
-   [ ] Session persistence
-   [ ] TLS termination
-   [ ] ALB
-   [ ] NLB
-   [ ] Kubernetes Service
-   [ ] Ingress
-   [ ] Failure scenarios
-   [ ] Load balancer troubleshooting

------------------------------------------------------------------------

# 15. Observability

## Observability Fundamentals

-   [ ] Metrics
-   [ ] Logs
-   [ ] Traces
-   [ ] Events
-   [ ] Golden signals
-   [ ] RED method
-   [ ] USE method
-   [ ] Correlation IDs
-   [ ] Transaction IDs
-   [ ] Alert quality
-   [ ] Noise reduction

## Prometheus

-   [ ] Architecture
-   [ ] Metrics
-   [ ] Targets
-   [ ] Exporters
-   [ ] PromQL
-   [ ] Labels
-   [ ] Recording rules
-   [ ] Alerting rules
-   [ ] Service discovery
-   [ ] Kubernetes monitoring

## Grafana

-   [ ] Datasources
-   [ ] Dashboards
-   [ ] Panels
-   [ ] Variables
-   [ ] Alerts
-   [ ] Kubernetes dashboards
-   [ ] Application dashboards

## Splunk

-   [ ] Index
-   [ ] Sourcetype
-   [ ] Source
-   [ ] Search
-   [ ] SPL
-   [ ] Field extraction
-   [ ] `rex`
-   [ ] `stats`
-   [ ] `timechart`
-   [ ] `transaction`
-   [ ] Correlation using transaction/request ID
-   [ ] Dashboards
-   [ ] Alerts
-   [ ] Production log troubleshooting

## Datadog

-   [ ] Metrics
-   [ ] Logs
-   [ ] APM
-   [ ] Monitors
-   [ ] Composite monitors
-   [ ] Dashboards
-   [ ] Tags
-   [ ] Service catalog concepts
-   [ ] SLOs
-   [ ] Alert thresholds
-   [ ] Monitor troubleshooting
-   [ ] Application health monitoring

## Dynatrace

-   [ ] Metrics
-   [ ] Logs
-   [ ] Traces
-   [ ] Service monitoring
-   [ ] Problem analysis
-   [ ] Dashboards
-   [ ] Alerting
-   [ ] Root-cause analysis

## Distributed Tracing

-   [ ] Trace
-   [ ] Span
-   [ ] Parent / child relationships
-   [ ] Trace ID
-   [ ] Span ID
-   [ ] Context propagation
-   [ ] OpenTelemetry
-   [ ] Application latency analysis

------------------------------------------------------------------------

# 16. SRE Fundamentals

-   [ ] What is SRE?
-   [ ] SRE vs DevOps
-   [ ] Reliability engineering
-   [ ] Availability
-   [ ] Reliability
-   [ ] Scalability
-   [ ] Performance
-   [ ] Resilience
-   [ ] SLIs
-   [ ] SLOs
-   [ ] SLAs
-   [ ] Error budgets
-   [ ] Burn rate
-   [ ] Toil
-   [ ] Automation
-   [ ] Capacity planning
-   [ ] Reliability trade-offs

## Common Metrics

-   [ ] Availability
-   [ ] Latency
-   [ ] Error rate
-   [ ] Throughput
-   [ ] MTTR
-   [ ] MTTD
-   [ ] MTBF
-   [ ] Change failure rate

------------------------------------------------------------------------

# 17. Incident Management

-   [ ] P1 incident
-   [ ] P2 incident
-   [ ] P3 incident
-   [ ] P4 incident
-   [ ] Incident commander
-   [ ] Technical lead
-   [ ] Communications lead
-   [ ] Stakeholder communication
-   [ ] Incident bridge
-   [ ] Triage
-   [ ] Mitigation
-   [ ] Recovery
-   [ ] RCA
-   [ ] Postmortem
-   [ ] Corrective actions
-   [ ] Preventive actions
-   [ ] Change management
-   [ ] CAB
-   [ ] Problem management
-   [ ] Known error
-   [ ] Runbooks

## Practice Scenarios

-   [ ] Deployment caused 5xx spike
-   [ ] Database latency increased
-   [ ] Kubernetes pods restarted
-   [ ] Certificate expired
-   [ ] Disk full
-   [ ] CPU saturation
-   [ ] Memory leak
-   [ ] DNS outage
-   [ ] Network latency
-   [ ] Service unavailable
-   [ ] Dependency outage
-   [ ] Load balancer health-check failure
-   [ ] CI/CD pipeline outage
-   [ ] Monitoring outage

------------------------------------------------------------------------

# 18. Production Readiness

For every service, understand:

-   [ ] Architecture documented
-   [ ] Dependencies documented
-   [ ] Health checks
-   [ ] Readiness / liveness
-   [ ] Logging
-   [ ] Metrics
-   [ ] Tracing
-   [ ] Alerts
-   [ ] Dashboard
-   [ ] SLI/SLO
-   [ ] Capacity planning
-   [ ] Autoscaling
-   [ ] Security
-   [ ] Secrets management
-   [ ] Backup
-   [ ] Disaster recovery
-   [ ] Rollback
-   [ ] Runbook
-   [ ] On-call process
-   [ ] Incident procedure
-   [ ] Deployment strategy
-   [ ] Change management
-   [ ] Cost visibility

------------------------------------------------------------------------

# 19. Security

-   [ ] IAM
-   [ ] Least privilege
-   [ ] Secrets management
-   [ ] TLS
-   [ ] Certificates
-   [ ] Kubernetes RBAC
-   [ ] NetworkPolicy
-   [ ] Container security
-   [ ] Image scanning
-   [ ] Vulnerability management
-   [ ] Dependency scanning
-   [ ] SAST
-   [ ] DAST concepts
-   [ ] Security groups
-   [ ] Private networking
-   [ ] Encryption at rest
-   [ ] Encryption in transit
-   [ ] Audit logs
-   [ ] AWS CloudTrail concepts
-   [ ] Key management concepts

------------------------------------------------------------------------

# 20. OAuth / OIDC / Keycloak

This is a key gap for the KNIME-style role.

-   [ ] Authentication vs authorization
-   [ ] OAuth 2.0
-   [ ] OpenID Connect
-   [ ] Identity Provider
-   [ ] Client
-   [ ] Resource server
-   [ ] Access token
-   [ ] Refresh token
-   [ ] ID token
-   [ ] JWT
-   [ ] Claims
-   [ ] Scopes
-   [ ] Roles
-   [ ] Authorization Code flow
-   [ ] Client Credentials flow
-   [ ] PKCE
-   [ ] Keycloak architecture
-   [ ] Realms
-   [ ] Clients
-   [ ] Users
-   [ ] Roles
-   [ ] Groups
-   [ ] Identity providers
-   [ ] Keycloak with Kubernetes
-   [ ] Troubleshoot authentication failures

------------------------------------------------------------------------

# 21. PostgreSQL

-   [ ] Database fundamentals
-   [ ] Tables
-   [ ] Indexes
-   [ ] Primary keys
-   [ ] Foreign keys
-   [ ] Joins
-   [ ] Transactions
-   [ ] ACID
-   [ ] Isolation levels
-   [ ] Locks
-   [ ] Connection pools
-   [ ] Max connections
-   [ ] Slow queries
-   [ ] Query plans
-   [ ] `EXPLAIN`
-   [ ] CPU issues
-   [ ] Memory issues
-   [ ] Disk issues
-   [ ] Backup
-   [ ] Restore
-   [ ] Replication concepts
-   [ ] High availability
-   [ ] Application-to-database troubleshooting

------------------------------------------------------------------------

# 22. Cost Optimization

-   [ ] AWS cost model
-   [ ] EC2 rightsizing
-   [ ] EBS optimization
-   [ ] S3 lifecycle policies
-   [ ] Unused resources
-   [ ] NAT Gateway cost
-   [ ] Data transfer costs
-   [ ] RDS sizing
-   [ ] EKS cost
-   [ ] Kubernetes resource requests
-   [ ] Autoscaling
-   [ ] Spot instances concepts
-   [ ] Reserved Instances / Savings Plans concepts
-   [ ] Cost allocation tags
-   [ ] AWS Cost Explorer
-   [ ] Cost anomaly detection concepts

------------------------------------------------------------------------

# 23. Scalability

-   [ ] Horizontal scaling
-   [ ] Vertical scaling
-   [ ] Stateless services
-   [ ] Stateful services
-   [ ] Caching
-   [ ] Load balancing
-   [ ] Database scaling
-   [ ] Read replicas
-   [ ] Connection pooling
-   [ ] Queue-based architecture
-   [ ] Async processing
-   [ ] Backpressure
-   [ ] Rate limiting
-   [ ] Capacity planning
-   [ ] Bottleneck identification
-   [ ] Performance testing

------------------------------------------------------------------------

# 24. High Availability / Disaster Recovery

-   [ ] Availability Zones
-   [ ] Multi-AZ
-   [ ] Redundancy
-   [ ] Failover
-   [ ] Health checks
-   [ ] RTO
-   [ ] RPO
-   [ ] Backup
-   [ ] Restore
-   [ ] DR strategies
-   [ ] Pilot light
-   [ ] Warm standby
-   [ ] Active-active
-   [ ] Active-passive
-   [ ] Cross-region concepts
-   [ ] Disaster recovery testing

------------------------------------------------------------------------

# 25. Platform Engineering

-   [ ] Internal developer platform concepts
-   [ ] Golden paths
-   [ ] Self-service infrastructure
-   [ ] Standardized CI/CD
-   [ ] Reusable Terraform modules
-   [ ] Reusable Helm charts
-   [ ] Kubernetes platform standards
-   [ ] Observability standards
-   [ ] Security guardrails
-   [ ] Developer experience
-   [ ] Platform reliability
-   [ ] Automation-first mindset

------------------------------------------------------------------------

# 26. Reliability Standards

-   [ ] Define SLOs
-   [ ] Standardize health checks
-   [ ] Standardize alerts
-   [ ] Standardize dashboards
-   [ ] Standardize logging
-   [ ] Standardize deployment strategy
-   [ ] Standardize rollback
-   [ ] Standardize incident response
-   [ ] Standardize runbooks
-   [ ] Reduce alert noise
-   [ ] Reduce toil
-   [ ] Automate repetitive operations

------------------------------------------------------------------------

# 27. Cross-Team Engineering

-   [ ] Working with developers
-   [ ] Working with QA
-   [ ] Working with security
-   [ ] Working with networking
-   [ ] Working with database teams
-   [ ] Working with product teams
-   [ ] Stakeholder communication
-   [ ] Incident communication
-   [ ] Technical documentation
-   [ ] Knowledge sharing
-   [ ] Mentoring
-   [ ] Engineering standards
-   [ ] Technical decision-making
-   [ ] Handling disagreements professionally

------------------------------------------------------------------------

# 28. Automation-First Mindset

For repetitive work, ask:

> Can this be monitored, scripted, automated, or prevented?

Practice automating:

-   [ ] Log cleanup
-   [ ] Disk checks
-   [ ] Certificate expiry checks
-   [ ] Service health checks
-   [ ] Kubernetes health checks
-   [ ] AWS resource checks
-   [ ] Deployment validation
-   [ ] Failed-pod reports
-   [ ] Restart detection
-   [ ] Alert enrichment
-   [ ] Cost reports
-   [ ] Backup verification
-   [ ] Compliance checks

------------------------------------------------------------------------

# 29. 3-Month Capstone Project

Build one production-style platform that ties the entire roadmap
together.

## Architecture

``` text
Developer
   |
   v
Git Repository
   |
   v
Jenkins CI
   |
   +--> Unit Tests
   +--> Security Scan
   +--> Docker Build
   +--> Push to ECR
   |
   v
Helm
   |
   v
EKS
   |
   +--> Deployment
   +--> Service
   +--> Ingress / ALB
   |
   v
Application
   |
   +--> PostgreSQL / RDS
   |
   +--> Prometheus
   +--> Grafana
   +--> Datadog
   +--> CloudWatch
```

## Infrastructure

-   [ ] Terraform VPC
-   [ ] Terraform subnets
-   [ ] Terraform IAM
-   [ ] Terraform EKS
-   [ ] Terraform ECR
-   [ ] Terraform RDS
-   [ ] Terraform monitoring resources
-   [ ] Remote Terraform state

## Application

-   [ ] Build a small Spring Boot or FastAPI service
-   [ ] Health endpoint
-   [ ] Readiness endpoint
-   [ ] Database integration
-   [ ] Structured logging
-   [ ] Metrics
-   [ ] Dockerfile
-   [ ] Unit tests

## CI/CD

-   [ ] Git repository
-   [ ] Jenkins pipeline
-   [ ] Test stage
-   [ ] Build stage
-   [ ] Security scan
-   [ ] Docker image
-   [ ] Push to ECR
-   [ ] Helm deployment
-   [ ] Rollback
-   [ ] Optional Argo CD GitOps flow

## Observability

-   [ ] Prometheus
-   [ ] Grafana
-   [ ] Datadog
-   [ ] CloudWatch
-   [ ] Logs
-   [ ] Metrics
-   [ ] Alerts
-   [ ] Dashboard
-   [ ] Trace / correlation ID

## Python Automation

-   [ ] Health-check script
-   [ ] AWS resource checker
-   [ ] Kubernetes diagnostics script
-   [ ] Deployment validator
-   [ ] Certificate expiry checker

## Security

-   [ ] IAM least privilege
-   [ ] Kubernetes RBAC
-   [ ] Secrets
-   [ ] TLS
-   [ ] Container image scan
-   [ ] Network controls
-   [ ] Keycloak / OIDC integration

------------------------------------------------------------------------

# 30. Deliberately Break the Platform

This is critical for becoming interview-ready.

For every failure, document:

**Symptom → Investigation → Evidence → Root Cause → Immediate Mitigation
→ Permanent Fix → Prevention**

Break and troubleshoot:

-   [ ] Bad deployment
-   [ ] Broken image
-   [ ] Readiness probe failure
-   [ ] Liveness probe failure
-   [ ] OOMKilled
-   [ ] CPU saturation
-   [ ] Memory saturation
-   [ ] Disk full
-   [ ] Node NotReady
-   [ ] Service failure
-   [ ] Ingress failure
-   [ ] DNS failure
-   [ ] NetworkPolicy issue
-   [ ] Database connection failure
-   [ ] Database latency
-   [ ] Certificate expiry
-   [ ] IAM AccessDenied
-   [ ] ECR permission failure
-   [ ] Terraform drift
-   [ ] Terraform failure
-   [ ] Jenkins agent failure
-   [ ] Jenkins pipeline failure
-   [ ] Argo CD sync failure
-   [ ] Monitoring failure
-   [ ] Alert storm
-   [ ] High application latency

------------------------------------------------------------------------

# 31. Interview Readiness

For each major topic, be able to answer at five levels:

### Level 1 --- Understand

-   [ ] Can I explain what it is?

### Level 2 --- Build

-   [ ] Can I create it myself?

### Level 3 --- Break

-   [ ] Can I deliberately cause a failure?

### Level 4 --- Troubleshoot

-   [ ] Can I investigate it using commands, logs, metrics and traces?

### Level 5 --- Interview

-   [ ] Can I explain the issue clearly in 60--90 seconds?

### Level 6 --- CV Evidence

-   [ ] Can I honestly point to a project, lab, production experience,
    or GitHub evidence?

------------------------------------------------------------------------

# 32. Final 3-Month Outcome

By the end of the roadmap, the target should be:

-   [ ] Strong AWS fundamentals
-   [ ] Strong EKS/Kubernetes troubleshooting
-   [ ] Strong Linux troubleshooting
-   [ ] Strong Terraform
-   [ ] Strong CI/CD
-   [ ] Practical Jenkins
-   [ ] Practical GitOps / Argo CD
-   [ ] Practical Helm
-   [ ] Practical Docker
-   [ ] Practical Python automation
-   [ ] Practical Bash
-   [ ] Strong observability
-   [ ] Strong Splunk
-   [ ] Strong Datadog
-   [ ] Working Dynatrace knowledge
-   [ ] Prometheus/Grafana
-   [ ] SRE fundamentals
-   [ ] Incident management
-   [ ] Production readiness
-   [ ] Security fundamentals
-   [ ] OAuth/OIDC/Keycloak basics
-   [ ] PostgreSQL troubleshooting
-   [ ] Azure working knowledge
-   [ ] Cost optimization awareness
-   [ ] HA/DR understanding
-   [ ] Platform engineering understanding
-   [ ] Production-style GitHub project
-   [ ] Multiple troubleshooting case studies
-   [ ] Strong SRE/DevOps interview stories

------------------------------------------------------------------------

## Target CV Niche After the Roadmap

**SRE / Cloud Platform Engineer**

**AWS \| Kubernetes/EKS \| Terraform \| CI/CD \| Python/Bash Automation
\| Observability \| Production Reliability**

Primary depth: - AWS - Kubernetes/EKS - Linux - Terraform -
Jenkins/CI/CD - Python/Bash - Observability - Incident response

Secondary depth: - Helm - Docker - Git - Argo CD/GitOps - PostgreSQL -
Security - SLO/SLI - HA/DR - Cost optimization

Gap-closing knowledge: - Azure - OAuth/OIDC - Keycloak - Kubernetes
Operators - CloudFormation

Nice-to-have: - Go - Advanced distributed systems - Advanced Kubernetes
operator development
