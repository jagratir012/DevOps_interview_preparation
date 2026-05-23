# 🚀 DevOps Interview Roadmap for 5 Years Experience

A complete **Senior DevOps / SRE / Platform Engineering Interview Preparation Repository** for engineers targeting:

- FAANG Companies
- Product-Based Companies
- High Scale Startups
- 40+ LPA Roles

This repository contains:
- Linux Deep Dive
- Kubernetes Troubleshooting
- AWS Architecture
- Docker
- Terraform
- CI/CD
- Monitoring & Observability
- DevOps System Design
- Production Scenarios
- Behavioral Questions
- Mock Interviews
- Senior-Level Interview Questions & Answers

---

# 👨‍💻 Who Is This Repository For?

This repository is designed for:
- DevOps Engineers
- SRE Engineers
- Platform Engineers
- Cloud Engineers
- Backend Engineers transitioning into DevOps/SRE

### Experience Level
- 4–8 Years

---

# 🎯 Main Goal

Prepare for:
- Senior DevOps Engineer
- Site Reliability Engineer (SRE)
- Platform Engineer
- Infrastructure Engineer

Target Salary:
- 40+ LPA

---

# 📚 Repository Structure

```bash
devops-interview-roadmap/
│
├── linux/
├── kubernetes/
├── aws/
├── terraform/
├── docker/
├── cicd/
├── monitoring/
├── system-design/
├── sre/
├── production-scenarios/
├── behavioral/
├── mock-interviews/
└── README.md
```

---

# 🐧 linux/

# Important Topics

## Linux Fundamentals
- Process Management
- Systemd
- SSH
- Permissions
- File Systems
- Memory Management
- CPU Scheduling

## Networking Commands
```bash
netstat
ss
tcpdump
curl
dig
ping
traceroute
```

## Important Linux Commands
```bash
top
htop
ps -ef
grep
awk
sed
journalctl
df -h
du -sh
iostat
vmstat
```

---

# Important Interview Questions

## Q1. Difference between soft link and hard link?

### Answer
- Hard link points to inode
- Soft link points to file path
- Hard link survives original file deletion
- Soft link breaks if original file deleted

---

## Q2. What will you do if CPU becomes 100%?

### Answer
1. Identify process
```bash
top
htop
ps -ef
```

2. Analyze threads
3. Check traffic spike
4. Check cron jobs
5. Capture logs
6. Mitigate using scaling or restart
7. Perform RCA

---

# ☸️ kubernetes/

# Important Topics

## Kubernetes Core
- Pod
- Deployment
- Service
- ConfigMap
- Secret
- Namespace

## Advanced Kubernetes
- RBAC
- HPA
- StatefulSet
- DaemonSet
- Taints/Tolerations
- Affinity

## Networking
- Ingress
- CoreDNS
- kube-proxy
- CNI

## Troubleshooting
```bash
kubectl describe pod
kubectl logs
kubectl exec
kubectl top pod
kubectl get events
```

---

# Important Interview Questions

## Q1. Pod is in CrashLoopBackOff. How will you debug?

### Answer
1. Check pod events
```bash
kubectl describe pod <pod>
```

2. Check logs
```bash
kubectl logs <pod> --previous
```

3. Verify:
- env variables
- secrets
- image version
- memory limits
- DB connection

4. Rollback deployment if needed

---

## Q2. Difference between Deployment and StatefulSet?

### Answer

### Deployment
- Stateless applications
- Random pod names
- Independent pods

### StatefulSet
- Stateful applications
- Stable network identity
- Ordered deployment

Used for:
- Kafka
- MongoDB
- Elasticsearch

---

# ☁️ aws/

# Important Topics

## AWS Core Services
- EC2
- EKS
- VPC
- IAM
- Route53
- ALB/NLB
- CloudWatch
- Auto Scaling

---

# Important Interview Questions

## Q1. Difference between Security Group and NACL?

### Answer

### Security Group
- Instance level
- Stateful

### NACL
- Subnet level
- Stateless

---

## Q2. Website is down behind ALB. What will you check?

### Answer
1. Target group health
2. Security group
3. EC2 health
4. Route table
5. NACL
6. CloudWatch metrics

---

# 🐳 docker/

# Important Topics

- Docker Architecture
- Dockerfile
- Multi-stage build
- Networking
- Volumes
- Image optimization

---

# Important Interview Questions

## Q1. Difference between CMD and ENTRYPOINT?

### Answer

### CMD
Default command

### ENTRYPOINT
Fixed executable

ENTRYPOINT cannot be overridden easily.

---

# 🌍 terraform/

# Important Topics

- Providers
- Resources
- Variables
- Outputs
- State Management
- Remote Backend
- Modules

---

# Important Interview Questions

## Q1. Why remote backend is important?

### Answer
- Shared state
- Team collaboration
- State locking
- Prevent corruption

---

## Q2. What is Terraform drift?

### Answer
Difference between:
- actual infrastructure
- terraform state

Occurs when infra modified manually.

---

# 🔄 cicd/

# Important Topics

- Jenkins
- GitHub Actions
- GitLab CI
- Blue-Green Deployment
- Canary Deployment
- Rollback Strategy

---

# Important Interview Questions

## Q1. Pipeline suddenly fails. How will you debug?

### Answer
1. Check agent availability
2. Verify credentials
3. Check logs
4. Validate dependencies
5. Check disk space

---

## Q2. Difference between Blue-Green and Canary deployment?

### Answer

### Blue-Green
Two environments
Instant switch

### Canary
Gradual traffic shifting
Safer for production

---

# 📊 monitoring/

# Important Topics

- Prometheus
- Grafana
- ELK Stack
- Loki
- Alertmanager

---

# Important Interview Questions

## Q1. What is cardinality issue in Prometheus?

### Answer
Too many unique labels causing:
- high memory usage
- performance issues

---

## Q2. Difference between metrics and logs?

### Answer

### Metrics
Numerical data
Good for monitoring

### Logs
Detailed events
Good for debugging

---

# 🏗️ system-design/

# Important Topics

## Design These Systems
- Scalable CI/CD Platform
- Kubernetes Platform
- Observability Platform
- Multi-region Infrastructure

---

# Important Interview Questions

## Q1. How will you design scalable CI/CD platform?

### Answer
Must include:
- Git webhook
- Build agents
- Artifact repository
- Container registry
- Deployment strategy
- Rollback mechanism
- Monitoring

---

# 🔥 sre/

# Important Topics

- SLA
- SLO
- Error Budget
- RCA
- Incident Management

---

# Important Interview Questions

## Q1. Difference between SLA and SLO?

### Answer

### SLA
Customer agreement

### SLO
Internal reliability target

---

## Q2. How will you handle production outage?

### Answer
1. Reduce customer impact
2. Create bridge call
3. Rollback/mitigate
4. Investigate RCA
5. Prevent recurrence

---

# 🚨 production-scenarios/

# Important Production Scenarios

## Scenario 1
Pods crashing after deployment

## Scenario 2
CPU suddenly spikes

## Scenario 3
Memory leak

## Scenario 4
503 errors in production

## Scenario 5
Auto scaling not working

## Scenario 6
EKS nodes not joining cluster

---

# 🧠 behavioral/

# Most Asked Behavioral Questions

## Q1. Tell me about major outage you handled?

### Answer Structure
- Situation
- Impact
- Action
- Resolution
- Learning

---

## Q2. Tell me about conflict with developer?

### Answer
- collaborative approach
- data-driven discussion
- customer-first mindset

---

# 🎯 mock-interviews/

# Mock Interview Topics

## Linux
- CPU spike
- Disk full
- High memory

## Kubernetes
- Pod pending
- DNS issue
- Ingress issue

## AWS
- ALB issue
- IAM issue
- VPC issue

## CI/CD
- Deployment failure
- Rollback strategy

---

# 📈 Daily Interview Preparation Plan

| Activity | Duration |
|---|---|
| Linux + K8s | 1.5 Hours |
| AWS + Terraform | 1 Hour |
| Scenario Practice | 1 Hour |
| Mock Interview | 30 Minutes |
| Revision | 30 Minutes |

---

# 🔥 Most Important Skills for 40+ LPA

| Skill | Priority |
|---|---|
| Kubernetes Troubleshooting | EXTREME |
| Linux Debugging | EXTREME |
| AWS Architecture | HIGH |
| Incident Handling | HIGH |
| CI/CD Design | HIGH |
| System Design | HIGH |
| Networking | HIGH |

---

# 🏆 Senior Engineer Mindset

Always answer using:

1. Impact
2. Investigation
3. Mitigation
4. RCA
5. Prevention

---

# 🚀 Final Goal

Become confident in:
- Production troubleshooting
- Kubernetes debugging
- AWS architecture
- Incident handling
- System design
- Reliability engineering

---

# ⭐ Contribute

Feel free to contribute:
- Real production scenarios
- Kubernetes troubleshooting guides
- AWS architecture notes
- DevOps interview questions
- System design documents

---

# 📜 License

MIT License

---

# 🙌 Happy Learning

Keep building.
Keep debugging.
Keep scaling.

🚀
