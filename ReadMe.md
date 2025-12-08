# Shivam Chaubey
**Backend & Infrastructure Engineer** | Building systems that scale, fail gracefully, and cost less

![Go](https://img.shields.io/badge/Go-00ADD8?style=flat&logo=go&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat&logo=kubernetes&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat&logo=amazon-aws&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=flat&logo=terraform&logoColor=white)

I write Go, automate infrastructure, and debug distributed systems at 3 AM (for fun, unfortunately).

---

## What I'm Building Right Now

**Improving my own projects** to understand the "why" behind every decision.
Currently writing about why HPA fails for queue-based workloads and when you 
should (and shouldn't) build custom K8s controllers.

[→ Read my latest](https://shivamchaubey.live/blog/building-a-kubernetes-monitoring-stack-from-scratch-phase-1/)



---

## Recent Projects

### Custom Kubernetes Autoscaler
**Go • Prometheus • K8s Client-go** | [Code](https://github.com/shivamchaubey027/Kubernetes-Monitoring-and-Autoscaling-System) | [Deep Dive](https://shivamchaubey.live/blog/building-a-kubernetes-monitoring-stack-from-scratch-phase-1/)

Built a controller that scales pods based on *business metrics* (queue depth, request rates) instead of CPU/memory. HPA doesn't cut it when your bottleneck isn't resources.

- Reduced Docker images 98% (1.2GB → 20MB) with multi-stage builds
- Integrated PromQL for real-time metric queries
- Handles ~500 pods across 3 clusters without breaking a sweat

**The interesting problem:** Preventing scale flapping during traffic bursts without introducing lag.

### Multi-Region Disaster Recovery Platform
**AWS • Terraform • RDS** | [Code](https://github.com/shivamchaubey027/Multi-Region-Disaster-Recovery-Platform-with-Automated-Failover)

Architected a resilient setup that survives entire AWS region failures.

- RTO: <15 minutes (tested, not theoretical)
- RPO: <5 minutes via RDS cross-region replication
- Automated failover with Terraform state management

**The trade-off:** Cost vs availability. Documented every decision in technical logs.

### Kubernetes Cost Estimator
**Go • PostgreSQL • K8s API** | [Code](https://github.com/shivamchaubey027/k8s-cost-optimizer)

Real-time cost visibility for K8s clusters. Because "just add more pods" isn't a scaling strategy.

- Parses raw K8s resource units (100m CPU, 128Mi RAM) → actual cloud spend
- REST API for teams to query their burn rate
- Integrated AWS pricing models for accurate estimates

---

## What I Care About

**Reliability over features**  
I'd rather ship one thing that works under load than ten things that break in production.

**Observability from day one**  
If you can't measure it, you can't debug it. Prometheus, Grafana, and structured logging aren't optional.

**Infrastructure as actual code**  
Not YAML copy-paste. Modular Terraform, tested pipelines, version-controlled everything.

**Learning in public**  
I write about what I build and what breaks. [Read my blog →](https://shivamchaubey.live)

---

## Current Explorations

- SLIs, SLOs, and error budgets (reading Google SRE book)
- Writing Kubernetes operators that don't eat your CPU
- Redis Lua scripts for atomic distributed operations
- eBPF for low-level observability (still wrapping my head around this)

---

## Tech I Work With
**Languages:** Go (primary), Python  
**Cloud & Orchestration:** AWS, Kubernetes, Terraform, Docker  
**Observability:** Prometheus, Grafana, PromQL, custom exporters  
**Databases:** PostgreSQL, Redis  
**Tools:** Git, GitHub Actions, Linux internals

---

## Let's Connect

I'm always down to talk about distributed systems, Kubernetes internals, or why your monitoring setup is lying to you.

📧 shivamchaubey027@gmail.com  
🔗 [LinkedIn](https://linkedin.com/in/shivamchaubey027) | [Portfolio](https://shivamchaubey.live) | [Blog](https://shivamchaubey.live/blog)

---

*Building from Mumbai, India. Open to remote backend/platform engineering opportunities.*
