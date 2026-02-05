---
title: "PIMCO: GitOps for High-Performance Computing"
description: "Architected Kubernetes-based HPC platform with GitOps and Kafka for a global investment management firm."
date: 2018-08-01
tags: ["GitOps", "Kubernetes", "Financial Services"]
result: "6,000% efficiency gain"
role: "Sr. DevOps Engineer"
tech: ["Kubernetes", "GitOps", "Kafka", "Okta", "Auth0"]
featured: true
order: 1
---

## The Challenge

PIMCO, one of the world's largest investment management firms, needed a high-performance computing platform capable of supporting complex financial calculations at scale. The existing infrastructure couldn't keep pace with the demands of managing over a trillion dollars in assets.

## The Approach

Architected a Kubernetes-based HPC solution with a dual authentication strategy: Okta for infrastructure access and Auth0 for service-level authentication. Implemented GitOps practices alongside Kafka for event-driven processing.

### Key Decisions

- **Kubernetes-centric architecture** — Container orchestration provided the flexibility and scalability required for HPC workloads
- **GitOps workflow** — All infrastructure and application changes flow through Git, providing audit trails and rollback capabilities critical in financial services
- **Kafka integration** — Event-driven architecture enabled real-time data processing at scale

## The Result

The platform achieved a **6,000% efficiency gain** in computational throughput. More importantly, the solution proved durable — it continues to support **$1.4 trillion in managed assets** years after initial deployment.

## Lessons Learned

In financial services, reliability isn't optional. The GitOps approach provided the change management rigor that compliance teams require while giving engineering teams the velocity they need. The dual-auth strategy — infrastructure vs. service authentication — has become a pattern I've reused in subsequent engagements.
