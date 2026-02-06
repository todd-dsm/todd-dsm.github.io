---
title: "Panasonic Avionics: Global Satellite Platform"
description: "Led multi-cloud migration (VMware to GCP/AWS) for global ground network supporting satellite comms and in-flight purchases. Reduced software delivery from two weeks to under 15 minutes."
date: 2018-08-01
tags: ["Cloud Migration", "Kubernetes", "Security", "GitOps", "AWS", "GCP"]
result: "4,800% efficiency gain"
role: "Cloud Infrastructure Architect"
tech: ["GKE", "EKS", "Istio", "HashiCorp Vault", "GitOps", "GCP", "AWS"]
featured: true
order: 1
---

## The Challenge

Panasonic Avionics operates the global ground network that powers inflight WiFi, entertainment systems, and transaction processing for airlines worldwide. The existing VMware-based infrastructure was limiting their ability to scale and iterate on their satellite communications platform.

Shipping a feature meant circular handoffs — dev → ops → QA → defects → repeat. Two weeks was optimistic.

## The Approach

Led a 3-person team through architecture and execution of a multi-cloud platform migration from on-premises VMware to GCP and AWS. The scope included satellite communications infrastructure, inflight WiFi systems, entertainment delivery, and payment transaction processing.

### Architecture Decisions

**Platform**
- **Kubernetes-centric design** — GKE provided the orchestration layer for containerized workloads across a globally distributed network
- **Istio service mesh** — Critical for securing service-to-service communication in a platform handling financial transactions and passenger data
- **HashiCorp Vault** — Centralized secrets management across a complex, distributed infrastructure
- **Solve once, replicate everywhere** — Once the cluster architecture was validated, every additional region became a multiplication problem, not an engineering problem

**Software Delivery**
- **GitOps practices** — All changes tracked in Git, enabling rapid iteration with full auditability
- **Automated Testing** — Validation gates ensured quality before deployment to production
- **Release Management** — Controlled rollouts across global regions with rollback capabilities

## The Result

The migration achieved a **4,800% efficiency gain** in software delivery — from two weeks to under 15 minutes.

With infrastructure distributed globally and automated tests on every push, teams became loosely coupled. Iterate locally, release globally — one operation.

## Lessons Learned

Migrating critical infrastructure isn't just a technical challenge — it's a trust exercise. The GitOps approach gave stakeholders visibility into every change, which built confidence to move faster. Security could be greatly improved without additional cost.

**Business Impact:** Gaining the capacity to deliver software globally within 15 minutes is how small advantages compound. Every iteration is a chance to learn, adjust, and pull further ahead.

**Social Impact:** Smooth delivery has a hidden benefit: less firefighting, less friction, less stress, more success and stronger teams. Success becomes repeatable — but only when teams stay together long enough to learn how.
